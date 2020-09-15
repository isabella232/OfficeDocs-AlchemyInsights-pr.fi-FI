---
title: Sähkö postin välitys ongelmien korjaaminen sähkö postia käyttävänä julkisissa kansioissa
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: da35ae4bd911fb75f23cc1c99aacbaa2392425dd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677925"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="f46e5-102">Sähkö postin välitys ongelmien korjaaminen sähkö postia käyttävänä julkisissa kansioissa</span><span class="sxs-lookup"><span data-stu-id="f46e5-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="f46e5-103">Jos ulkoiset lähettäjät eivät voi lähettää viestejä sähkö postia käyttäviin julkisiin kansioihin ja lähettäjät voivat saada virhe sanoman: **ei löytynyt (550 5.4.1)**, varmista, että yleisen kansion Sähkö posti toimi alue määritetään sisäisen välityksen toimi alueeksi hallitsevan toimi alueen sijaan:</span><span class="sxs-lookup"><span data-stu-id="f46e5-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="f46e5-104">Avaa [Exchange-hallinta keskus (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="f46e5-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="f46e5-105">Siirry kohtaan **sähkö postin kulun** \> **hyväksytyt toimi alueet**, valitse hyväksytty toimi alue ja valitse sitten **Muokkaa**.</span><span class="sxs-lookup"><span data-stu-id="f46e5-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="f46e5-106">Valitse avautuvassa ominaisuudet-sivulla, jos toimi alueen tyypiksi on valittu **määräävä**, muuta arvoksi **sisäinen rele** ja sitten **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="f46e5-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="f46e5-107">Jos ulkoiset lähettäjät saavat virhe ilmoituksen, **sinulla ei ole käyttö oikeutta (550 5.7.13)**, voit tarkastella yleisen kansion anonyymien käyttäjien käyttö oikeuksia suorittamalla seuraavan komennon [Exchange Online PowerShellissä](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) :</span><span class="sxs-lookup"><span data-stu-id="f46e5-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="f46e5-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Esimerkiksi `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .</span><span class="sxs-lookup"><span data-stu-id="f46e5-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="f46e5-109">Jos haluat, että ulkoiset käyttäjät voivat lähettää sähkö postia tähän julkiseen kansioon, lisää CreateItems-käyttö oikeus käyttäjälle anonyymi.</span><span class="sxs-lookup"><span data-stu-id="f46e5-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="f46e5-110">Esimerkiksi `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="f46e5-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
