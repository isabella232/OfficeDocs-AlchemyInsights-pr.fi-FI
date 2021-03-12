---
title: DKIM-tietuemuotoilun yleisimmät ongelmat
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746837"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>DKIM-tietuemuotoilun yleisimmät ongelmat

Useimmat DKIM:n määritysongelmat liittyvät virheellisiin DNS-tietueisiin.

Voit korjata DKIM-joukon ongelmat tarkistamalla, että DKIM CNAME -tietue **(ei** TXT-tietue) on muotoiltu oikein. Lisätietoja on ohjeaiheessa DKIM:n manuaalinen määritäminen [Office 365:ssä.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)

Jos tarvitset apua DNS-tietueiden yleisessä käyttöön, katso lisätietoja dns-tietueiden luominen missä tahansa [DNS-isännöintipalvelussa Office 365:tä varten.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

> [!NOTE]
> Kun olet luonut tai päivittänyt DKIM:n DNS-tietueet toimialueesi DNS-isännöintipalvelussa, sinun on odotettava DNS-tietueiden välitystä.
