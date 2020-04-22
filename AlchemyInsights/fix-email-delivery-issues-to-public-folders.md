---
title: Sähköpostin toimitusongelmien korjaaminen sähköpostia käyttäviin yleisiin kansioihin
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716349"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="06204-102">Sähköpostin toimitusongelmien korjaaminen sähköpostia käyttäviin yleisiin kansioihin</span><span class="sxs-lookup"><span data-stu-id="06204-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="06204-103">Jos ulkoiset lähettäjät eivät voi lähettää viestejä sähköpostia käyttäviin yleisiin kansioihin ja lähettäjät saavat virheen: **sitä ei löytynyt (550 5.4.1),** varmista, että yleisen kansion sähköpostitoimialue on määritetty sisäiseksi välitystoimialueeksi hallitsevan toimialueen sijaan:</span><span class="sxs-lookup"><span data-stu-id="06204-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="06204-104">Avaa [Exchange-hallintakeskus (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="06204-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="06204-105">Siirry **kohtaan Sähköpostin kulku** \> **Hyväksytyt toimialueet**, valitse hyväksytty toimialue ja valitse sitten **Muokkaa**.</span><span class="sxs-lookup"><span data-stu-id="06204-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="06204-106">Jos näyttöön avautuvalla ominaisuudet-sivulla toimialuetyypiksi on määritetty **Hallitseva,** muuta arvoksi **Sisäinen välitys** ja valitse sitten **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="06204-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="06204-107">Jos ulkoiset lähettäjät saavat **virheen, johon sinulla ei ole oikeuksia (550 5.7.13),** suorita seuraava komento [Exchange Online PowerShellissä,](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) niin näet anonyymien käyttäjien käyttöoikeudet yleiseen kansioon:</span><span class="sxs-lookup"><span data-stu-id="06204-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="06204-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Esimerkiksi `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="06204-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="06204-109">Jos haluat, että ulkoiset käyttäjät voivat lähettää sähköpostia tähän yleiseen kansioon, lisää CreateItems-käyttöoikeus anonyymille käyttäjälle.</span><span class="sxs-lookup"><span data-stu-id="06204-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="06204-110">Esimerkiksi `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="06204-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
