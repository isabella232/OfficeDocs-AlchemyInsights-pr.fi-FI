---
title: Päivittäinen sähkö postin enimmäismäärä ylittyi. Työn kulku on odotus tilassa.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731560"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Päivittäinen sähkö postin enimmäismäärä ylittyi. Työn kulku on odotus tilassa.

Tämä virhe saattaa tulla näyttöön seuraavissa tilanteissa:

- Sinulla on SharePoint Onlinen työn kulku, joka käyttää SharePoint 2010-tai SharePoint 2013-työn kulku ympäristön tyyppiä.
- Työn kulku on määritetty lähettämään mukautettu Sähkö posti viesti useammalle kuin 200-käyttäjälle kerralla, yli 10 000 käyttäjää päivässä tai yli 30 viestiä minuutissa.
- Kun suoritat työn kulun, sähkö posti viestiä ei lähetetä ja huomaat seuraavan ongelman:
    - Jos käytät työn kulkua SharePoint 2013-ympäristö tyypin kanssa, Selaa **työn kulun tila** -sivulle. Työn kulun tila-sivulla **sisäinen tila** -asetuksena on **aloitettu**ja tieto kuplassa **ei voi lähettää vastaanottajille**.

Voit kiertää tämän ongelman määrittämällä työn kulun lähettämään Sähkö posti viestejä ylittämättä [Exchange Online-lähettäjän rajoituksia](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Voit esimerkiksi käyttää keskeytystä työn kulussa, lähettää sähkö posti viestin Microsoft 365-ryhmään, jakeluun tai sähkö posti käyttöön, jossa on käytössä käyttö oikeus ryhmä, tai lähettää viestiä enintään 200 vastaanottajalla kerrallaan.


Lisä tietoja on seuraavassa [artikkelissa](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Aiheeseen liittyvät artikkelit
- [Työn kulun luominen](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ja Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 