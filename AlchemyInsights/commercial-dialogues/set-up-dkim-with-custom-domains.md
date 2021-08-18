---
title: DKIM:n luominen mukautettujen toimialueiden avulla
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: cb1f621dffc88464c339b55998efb5440cfd775c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332304"
---
# <a name="set-up-dkim-with-custom-domains"></a>DKIM:n luominen mukautettujen toimialueiden avulla

Sinun on julkaistava kaksi CNAME-tietuetta kullekin mukautetulle toimialueelle DNS:ssä. Voit tehdä tämän seuraavasti:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
**Huomautus:** **DomainGUID** on **.mail.protection.outlook.com-kohdan** vasemmalla puolella oleva teksti mukautetun toimialueen MX-tietueessa (esimerkiksi toimialueen contoso-com **contoso.com).** **InitialDomain** on toimialue, jota käytit rekisteröityessäsi Office 365 (esimerkiksi **contoso.onmicrosoft.com).**

Lisätietoja DNS-tietueista on kohdassa DNS-tietueiden luominen missä tahansa [DNS-isännöintipalvelussa Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)