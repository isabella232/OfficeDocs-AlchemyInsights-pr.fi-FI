---
title: PowerShellin käyttäminen käytäntöjen ja organisaation suhteiden jakamiseen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862085"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="5b3c6-102">PowerShellin käyttäminen käytäntöjen ja organisaation suhteiden jakamiseen</span><span class="sxs-lookup"><span data-stu-id="5b3c6-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="5b3c6-103">Organisaation suhteissa on tietoja : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) AND [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="5b3c6-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="5b3c6-104">Voit luoda jakamiskäytännön käyttämällä [New-SharingPolicy -toiminnolla](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="5b3c6-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="5b3c6-105">Jos haluat [käyttää jakamiskäytäntöä postilaatikkoon tai käyttäjään,](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) sinun on käytettävä [set-mailbox- ja get-mailbox-yhdistelmää](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) juuri luodun käytännön kanssa. [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox)</span><span class="sxs-lookup"><span data-stu-id="5b3c6-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="5b3c6-106">Jos haluat [muokata, poistaa käytöstä tai poistaa jakamiskäytännön,](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) sinun on käytettävä [Set-SharingPolicy-](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) ja [Remove-SharingPolicy -käytäntöä.](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy)</span><span class="sxs-lookup"><span data-stu-id="5b3c6-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="5b3c6-107">**Täydellinen käsitys tästä aiheesta lue:**</span><span class="sxs-lookup"><span data-stu-id="5b3c6-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="5b3c6-108">Jakaminen Exchange Onlinessa</span><span class="sxs-lookup"><span data-stu-id="5b3c6-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)