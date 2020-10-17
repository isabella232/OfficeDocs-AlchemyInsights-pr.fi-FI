---
title: 726 sähkö postin siirron estäminen
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
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478330"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Sähkö postin lähettämisen estäminen tai eston poistaminen

Jos haluat ottaa sähkö postin uudelleenohjauksen käyttöön tai poistaa sen käytöstä tietyssä posti laatikossa, katso [sähkö postin uudelleenohjauksen määrittäminen](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Vuokra ajan tasolla ulkoista lähetystä voidaan hallita lähtevällä roska posti käytännöllä. Voit tarkistaa lähtevän roska postin suodatus käytännöt tieto turva-ja yhteensopivuus keskuksesta [täällä](https://protection.office.com/antispam) tai käyttämällä [Get-Hostedoutboundspamfilttpolicy-komentoa](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).

Jos saat seuraavan virhe ilmoituksen: **"550 5.7.520 käyttö estetty, organisaatiosi ei salli ulkoista edelleenlähetystä"**, varmista, että käytännöt on määritetty niin, että ulkoinen automaattinen edelleensiirto on käytössä.

**Huomautus:** On suositeltavaa, että ulkoinen automaattinen siirto ei ole käytössä oletusarvoisessa lähtevän postin roska posti suodatus käytännössä ja että se on käytettävissä vain niitä käyttäjiä varten, jotka tarvitsevat ulkoista edelleenlähetystä luomalla mukautetun käytäntöjen näille käyttäjille. Lisä tietoja on artikkelissa [ulkoinen sähkö postin lähettäminen uudelleen Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)-sovelluksessa.