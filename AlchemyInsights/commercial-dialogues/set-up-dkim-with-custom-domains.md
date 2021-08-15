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
ms.openlocfilehash: bb19f0672a21ea8b99c433ad83db4d89536c9a1705245fd2a683471170ab51ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994807"
---
# <a name="set-up-dkim-with-custom-domains"></a>DKIM:n luominen mukautettujen toimialueiden avulla

Sinun on julkaistava kaksi CNAME-tietuetta kullekin mukautetulle DNS-toimialueelle. Voit tehdä tämän seuraavasti:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **DomainGUID** on **.mail.protection.outlook.com-kohdan** vasemmalla puolella oleva teksti mukautetun toimialueen MX-tietueessa (esimerkiksi toimialueen toimialueen contoso-com **contoso.com).** **InitialDomain** on toimialue, jota käytit rekisteröityessäsi Office 365 (esimerkiksi **contoso.onmicrosoft.com).**

Lisätietoja DNS-tietueista on kohdassa [DNS-tietueiden luominen missä tahansa DNS-isännöintipalvelussa Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)