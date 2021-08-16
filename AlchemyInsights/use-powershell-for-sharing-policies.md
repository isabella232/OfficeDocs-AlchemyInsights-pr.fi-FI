---
title: PowerShellin käyttäminen jakamiskäytännöille ja organisaatiosuhteille
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 48df03b1397b0e924aa878cea3d1cac07ca862c3636c1273d10f4841a03fddcf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998463"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>PowerShellin käyttäminen jakamiskäytännöille ja organisaatiosuhteille


Tutustu organisaatiosuhteiden yksityiskohtaisiin syntaksi- ja parametritietoihin komennoilla [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) ja [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Luo jakamiskäytäntö käyttämällä komentoa [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Jos haluat [käyttää jakamiskäytäntöä postilaatikolle tai käyttäjälle](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes), käytä juuri luodulle käytännölle komentoja [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) ja [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox). Jos haluat [muokata jakamiskäytäntöä, poistaa sen käytöstä tai poistaa sen kokonaan](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy), käytä komentoja [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) ja [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Katso lisätietoja tästä aiheesta artikkelista:**

[Jakaminen Exchange Onlinessa](https://docs.microsoft.com/exchange/sharing/sharing)