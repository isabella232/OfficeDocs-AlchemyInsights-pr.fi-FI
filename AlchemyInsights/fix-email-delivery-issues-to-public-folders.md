---
title: Korjaa sähköpostin toimitus ongelmat postijärjestelmän käynnistämät yleisiin kansioihin
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 45665f900014c52e6a920325b0a3b0f6f79fb72d
ms.sourcegitcommit: d1c1d5bcb52ba9083e8dd7603feb72436c5154c8
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/17/2019
ms.locfileid: "31910593"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="1bd5b-102">Korjaa sähköpostin toimitus ongelmat postijärjestelmän käynnistämät yleisiin kansioihin</span><span class="sxs-lookup"><span data-stu-id="1bd5b-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="1bd5b-103">Jos Ulkoiset lähettäjät voi lähettää viestejä, mail käytössä yleisissä kansioissa ja lähettäjien, näyttöön tulee virhesanoma: **(550 5.4.1) ei löytynyt**, Tarkista sähköposti toimialue on yleinen kansio on määritetty sisäinen relay toimialueen sijaan hallitseva toimialue:</span><span class="sxs-lookup"><span data-stu-id="1bd5b-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="1bd5b-104">Avaa [Exchange-hallintakeskukseen (AKV)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="1bd5b-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="1bd5b-105">Siirry **postin kulku** \> **hyväksytyt toimialueet**, hyväksytty toimialue ja valitse sitten **Muokkaa**.</span><span class="sxs-lookup"><span data-stu-id="1bd5b-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="1bd5b-106">Ominaisuudet-sivu, avautuu Jos **tärkeimmät**määritetään toimialueen laji, muuta **sisäistä relay** ja valitse sitten **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="1bd5b-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="1bd5b-107">Jos Ulkoiset lähettäjät tulee virhe, **sinulla ei ole oikeuksia (550 5.7.13)**, [Exchange Online-PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) julkisessa kansiossa anonyymeille käyttäjille oikeudet suorittamalla seuraavan komennon:</span><span class="sxs-lookup"><span data-stu-id="1bd5b-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="1bd5b-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Esimerkiksi `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="1bd5b-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="1bd5b-109">Ulkoiset käyttäjät voivat lähettää sähköpostia tähän yleiseen kansioon, Lisää CreateItems käyttöä oikealle anonyymi käyttäjä.</span><span class="sxs-lookup"><span data-stu-id="1bd5b-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="1bd5b-110">Esimerkiksi `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="1bd5b-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>