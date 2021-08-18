---
title: Ulkoisen automaattisen sähköpostin edelleenlähetysten estäminen tai eston poistaminen
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
ms.openlocfilehash: fe9e52023b809b38c43332a10a1184d114798cfe
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315871"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>Automaattisten sähköpostiviestien edelleenlähetysten estäminen tai eston poistaminen

Jos haluat ottaa sähköpostin edelleenlähetystä käyttöön tai poistaa sen käytöstä tietyssä postilaatikossa, katso sähköpostin [edelleenlähetysten määrittäminen.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Järjestelmänvalvojat voivat hallita organisaation ulkoista edelleenlähetystä [lähtevien roskapostikäytäntöjen avulla.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) Voit hallita lähtevän roskapostin käytäntöjä Microsoft 365 Defender-portaalissa <https://security.microsoft.com/antispam> [PowerShellin Get-HostedOutboundSpamFilterPolicy-cmdlet-komennolla](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) tai Exchange Online avulla.

Jos näyttöön tulee seuraava virhe: **"550 5.7.520 Käyttö estetty,** Organisaatiosi ei salli ulkoista edelleenlähetystä", varmista, että käytäntö on määritetty niin, että ulkoiset automaattisesti lähetetyt viestit otetaan käyttöön.

**Huomautus:** Suositellaan oletusarvoa Automaattinen **–**  Järjestelmä, jota hallitaan lähtevän liikenteen roskapostin oletussuodatuskäytännön Automaattiset edelleenlähetyssäännöt -asetuksella (automaattinen ulkoinen edelleenlähetys on estetty; sisäinen automaattinen edelleenlähetys toimii edelleen). Luo mukautettuja lähtevien roskapostisuodatuskäytäntöjä ja käytä arvoa **Käytössä – edelleenlähetys on** käytössä vain käyttäjille, jotka tarvitsevat ulkoista automaattista edelleenlähetystä. Lisätietoja on kohdassa Ulkoisen [sähköpostiviestin edelleenlähetysten määrittäminen Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)
