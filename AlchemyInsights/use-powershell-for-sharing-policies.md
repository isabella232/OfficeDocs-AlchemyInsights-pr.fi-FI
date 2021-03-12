---
title: PowerShellin käyttäminen jakamiskäytännöille ja organisaatiosuhteille
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: cd1d34e4dae474e61c799ca9234b2f18c718f27b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709463"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="a860e-102">PowerShellin käyttäminen jakamiskäytännöille ja organisaatiosuhteille</span><span class="sxs-lookup"><span data-stu-id="a860e-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="a860e-103">Tutustu organisaatiosuhteiden yksityiskohtaisiin syntaksi- ja parametritietoihin komennoilla [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) ja [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="a860e-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="a860e-104">Luo jakamiskäytäntö käyttämällä komentoa [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="a860e-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="a860e-105">Jos haluat [käyttää jakamiskäytäntöä postilaatikolle tai käyttäjälle](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes), käytä juuri luodulle käytännölle komentoja [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) ja [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox).</span><span class="sxs-lookup"><span data-stu-id="a860e-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="a860e-106">Jos haluat [muokata jakamiskäytäntöä, poistaa sen käytöstä tai poistaa sen kokonaan](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy), käytä komentoja [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) ja [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="a860e-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="a860e-107">**Katso lisätietoja tästä aiheesta artikkelista:**</span><span class="sxs-lookup"><span data-stu-id="a860e-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="a860e-108">Jakaminen Exchange Onlinessa</span><span class="sxs-lookup"><span data-stu-id="a860e-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)