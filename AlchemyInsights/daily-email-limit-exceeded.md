---
title: Päivittäinen Sähkö posti raja ylitetty. Työn kulku on keskeytetty.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053114"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Päivittäinen Sähkö posti raja ylitetty. Työn kulku on keskeytetty.

Tämä virhe voidaan vastaanottaa seuraavissa tilanteissa:

- Sinulla on SharePoint Onlinen työn kulku, joka käyttää SharePoint 2010-tai SharePoint 2013-työn kulku ympäristön tyyppiä.
- Työn kulku on määritetty lähettämään mukautettu Sähkö posti viesti yli 200 käyttäjälle kerrallaan, yli 10 000 vastaanottajaa päivässä tai yli 30 viestiä minuutissa.
- Kun suoritat työn kulun, sähkö posti viestiä ei lähetetä ja huomaat seuraavan ongelman:
    - Jos työn kulku käyttää SharePoint 2013-ympäristö tyyppiä, selaat **työn kulun tila** -sivua. Työn kulun tila-sivulla **sisäinen tila** on määritetty **aloiksi**ja tiedot-selite **ei voi lähettää vastaanottajalle**.

Voit kiertää tämän ongelman määrittämällä työn kulun lähettämään Sähkö posti viestejä ylittämättä [Exchange Online-lähettäjän rajoja](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Voit esimerkiksi käyttää keskeytystä työn kulussa, lähettää sähkö posti viestin Office 365-ryhmään, jakelu ryhmään tai sähkö posti käytössä olevaan suojaus ryhmään tai lähettää sanoman alle 200 vastaanottajalle kerrallaan.


Lisä tietoja on seuraavassa [artikkelissa](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Aiheeseen liittyvät artikkelit
- [Luo työn kulku](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ja Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 