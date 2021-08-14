---
title: DKIM-tietuemuotoilun yleisimmät ongelmat korjauksessa
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
ms.openlocfilehash: 5b3dc2338843906fbc7151322b82f304b4ed04b28d8ceb349f2705c309cdeae8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930058"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>DKIM-tietuemuotoilun yleisimmät ongelmat korjauksessa

Useimmat DKIM:n määritysongelmat liittyvät virheellisiin DNS-tietueisiin.

Voit korjata DKIM:n asennusongelmat tarkistamalla, että DKIM CNAME -tietue **(ei** TXT-tietue) on muotoiltu oikein. Lisätietoja on kohdassa [DKIM:n manuaalinen](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)Office 365.

Jos tarvitset apua DNS-tietueiden kanssa yleisesti, katso dns-tietueiden luominen missä tahansa [DNS-isännöintipalvelussa Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

> [!NOTE]
> Kun olet luonut tai päivittänyt DKIM:n DNS-tietueet toimialueesi DNS-isännöintipalvelussa, sinun on odotettava, kunnes DNS-tietueet välittyvät.
