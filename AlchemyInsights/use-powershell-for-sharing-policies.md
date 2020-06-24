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
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>PowerShellin käyttäminen käytäntöjen ja organisaation suhteiden jakamiseen


Organisaation suhteissa on tietoja : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) AND [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Voit luoda jakamiskäytännön käyttämällä [New-SharingPolicy -toiminnolla](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Jos haluat [käyttää jakamiskäytäntöä postilaatikkoon tai käyttäjään,](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) sinun on käytettävä [set-mailbox- ja get-mailbox-yhdistelmää](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) juuri luodun käytännön kanssa. [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) Jos haluat [muokata, poistaa käytöstä tai poistaa jakamiskäytännön,](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) sinun on käytettävä [Set-SharingPolicy-](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) ja [Remove-SharingPolicy -käytäntöä.](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy)

**Täydellinen käsitys tästä aiheesta lue:**

[Jakaminen Exchange Onlinessa](https://docs.microsoft.com/exchange/sharing/sharing)