---
title: Määrittää tai muuttaa yleisen kansiokäyttöoikeudet
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: d1554e8a63455f3549044e526183c0e8709f2631
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/22/2019
ms.locfileid: "30767281"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="fcfed-102">Käyttöoikeudet ja julkiset kansiot</span><span class="sxs-lookup"><span data-stu-id="fcfed-102">Permissions and Public Folders</span></span>

<span data-ttu-id="fcfed-103">Yleiset kansiot Outlook, Exchange-hallintakeskukseen (AKV), voit muuttaa käyttöoikeuksia tai PowerShell:</span><span class="sxs-lookup"><span data-stu-id="fcfed-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="fcfed-104">Outlookin ohjeet [napsauttamalla tätä](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span><span class="sxs-lookup"><span data-stu-id="fcfed-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="fcfed-105">AKV-kohdassa [Tässä artikkelissa](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) .</span><span class="sxs-lookup"><span data-stu-id="fcfed-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span></span> <span data-ttu-id="fcfed-106">Napsauttamalla [tätä](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx) voit siirtyä AKV.</span><span class="sxs-lookup"><span data-stu-id="fcfed-106">You can click [here](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx) to navigate to EAC.</span></span> 
    
- <span data-ttu-id="fcfed-107">PowerShell Katso [tämän artikkelin](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) käyttämällä Lisää-PublicFolderClientPermission-komentosovelmalla.</span><span class="sxs-lookup"><span data-stu-id="fcfed-107">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span></span> <span data-ttu-id="fcfed-108">Jos tarvitset ohjeita yhteyden muodostamiseen Exchange Powershell, napsauta [tätä](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span><span class="sxs-lookup"><span data-stu-id="fcfed-108">If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="fcfed-109">Jos **Ulkoiset käyttäjät eivät pysty lähettämään sähköpostit sähköpostin käytössä yleiseen kansioon**, syy saattaa yleisestä kansiosta puuttuu käyttöoikeudet edellyttää ulkoisen sähköpostin toimittamista varten.</span><span class="sxs-lookup"><span data-stu-id="fcfed-109">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery.</span></span> <span data-ttu-id="fcfed-110">Voit korjata tämän käyttämällä Outlookin ohjeet [tähän](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)tai PowerShell-ohjeet [tähän](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span><span class="sxs-lookup"><span data-stu-id="fcfed-110">You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

