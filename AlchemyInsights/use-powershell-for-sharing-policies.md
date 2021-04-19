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
ms.openlocfilehash: 9c52b876160f9577e6cefe7644c29d6fdf3b23fd
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826052"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>PowerShellin käyttäminen jakamiskäytännöille ja organisaatiosuhteille


Tutustu organisaatiosuhteiden yksityiskohtaisiin syntaksi- ja parametritietoihin komennoilla [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) ja [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Luo jakamiskäytäntö käyttämällä komentoa [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Jos haluat [käyttää jakamiskäytäntöä postilaatikolle tai käyttäjälle](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes), käytä juuri luodulle käytännölle komentoja [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) ja [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox). Jos haluat [muokata jakamiskäytäntöä, poistaa sen käytöstä tai poistaa sen kokonaan](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy), käytä komentoja [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) ja [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Katso lisätietoja tästä aiheesta artikkelista:**

[Jakaminen Exchange Onlinessa](https://docs.microsoft.com/exchange/sharing/sharing)