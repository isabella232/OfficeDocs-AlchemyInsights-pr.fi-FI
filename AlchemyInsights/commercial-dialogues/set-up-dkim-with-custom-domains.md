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
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745259"
---
# <a name="set-up-dkim-with-custom-domains"></a>DKIM:n luominen mukautettujen toimialueiden avulla

Sinun on julkaistava kaksi CNAME-tietuetta kutakin mukautettua toimialuetta varten DNS:ssä. Voit tehdä tämän seuraavasti:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **DomainGUID** on **.mail.protection.outlook.com-tietueen** vasemmalla puolella oleva teksti mukautetun toimialueen mukautetussa MX-tietueessa (esimerkiksi toimialueen toimialueen contoso-com **contoso.com).** **InitialDomain** on toimialue, jota käytit rekisteröityessäsi Office 365:tä (esimerkiksi **contoso.onmicrosoft.com).**

Lisätietoja DNS-tietueista on kohdassa [DNS-tietueiden luominen missä tahansa DNS-isännöintipalvelussa Office 365:tä varten.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)