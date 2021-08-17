---
title: 726 Sähköpostiviestien edelleenlähetysten estäminen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059629"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Sähköpostiviestien edelleenlähetysten estäminen tai eston poistaminen

Jos haluat ottaa sähköpostin edelleenlähetystä käyttöön tai poistaa sen käytöstä tietyssä postilaatikossa, katso sähköpostin [edelleenlähetysten määrittäminen.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Vuokraajan tasolla ulkoisen edelleenohjauksen hallinta tapahtuu lähtevän roskapostin käytännön avulla. Voit tarkistaa lähtevän roskapostin suodatuskäytännön [](https://protection.office.com/antispam) tietoturva- ja yhteensopivuuskeskuksesta täältä tai [käyttämällä Get-HostedOutboundSpamFilterPolicy-komentoa.](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)

Jos saat seuraavan virheilmoituksen: **"550 5.7.520** Käyttö estetty, Organisaatiosi ei salli ulkoista edelleenlähetystä", varmista, että käytäntö on määritetty sallimaan ulkoinen automaattinen edelleenlähetys.

**Huomautus:** On suositeltavaa, että Ulkoinen automaattinenforward -asetus on poissa käytöstä lähtevien roskapostien oletussuodatuskäytännön mukaisesti ja vain ulkoiset edelleenlähetystä tarvitsevat käyttäjät voivat ottaa sen käyttöön luomalla mukautetun käytännön kyseisille käyttäjille. Saat lisätietoja kohdasta Ulkoisen [sähköpostiviestin edelleenlähetysten määrittäminen Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)