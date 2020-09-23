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
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219852"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Sähkö postin lähettämisen estäminen tai eston poistaminen

Jos haluat ottaa sähkö postin uudelleenohjauksen käyttöön tai poistaa sen käytöstä tietyssä posti laatikossa, katso [sähkö postin uudelleenohjauksen määrittäminen](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Vuokra ajan tasolla ulkoista lähetystä voidaan hallita lähtevän roska postin vastaista käytäntöä käyttäen. Jos se on poistettu käytöstä tai se on automaattinen, se voi estää sähkö postin lähettämisen "550 5.7.520 käyttö estetty-virheen vuoksi, joten organisaatiosi ei salli ulkoista lähetystä"-virhe. Tämän jälkeen, jos siirto on tarkoitus estää, se on virhe, jonka käyttäjät näkevät.

Jos edelleenlähetystä ei estetä, varmista, että käytännöt on määritetty niin, että ulkoinen Autoforward on käytössä. Voit tarkistaa lähtevän roska postin suodatus käytännöt tieto turva-ja yhteensopivuus keskuksesta tai suorittamalla komennon Get-Hostedoutboundspamfilttpolicy | FL Name, Autofordingingmode. Jos haluat määrittää automaattisen edelleenkäytön eston, sama komento kertoo nyt käytännössä.

Huomautus: on suositeltavaa, että ulkoinen automaattinen edelleenlähetys on poistettu käytöstä lähtevien roska posti suodattimen oletus käytännöllä ja että se on käytettävissä vain niitä käyttäjiä varten, jotka tarvitsevat ulkoista edelleenlähetystä luomalla mukautetun käytäntöjen näille käyttäjille. Lisä tietoja on artikkelissa [ulkoinen sähkö postin lähettäminen uudelleen Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)-sovelluksessa.