---
title: Päivittäinen sähköpostirajoitus ylittyi. Työnkulku keskeytetään.
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
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914648"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Päivittäinen sähköpostirajoitus ylitetty. Työnkulku keskeytetään.

Tämä virhe voi tulla näyttöön seuraavissa tilanteissa:

- SharePoint Onlinessa on työnkulku, joka käyttää SharePoint 2010- tai SharePoint 2013 -työnkulkuympäristön tyyppiä.
- Työnkulku on määritetty lähettämään mukautettu sähköpostiviesti yli 200 käyttäjälle kerrallaan, yli 10 000 vastaanottajaa päivässä tai yli 30 viestiä minuutissa.
- Kun suoritat työnkulun, viestiä ei lähetetä ja huomaat seuraavan toiminnan:
    - Jos työnkulku käyttää SharePoint 2013 -käyttöympäristön tyyppiä, siirry Työnkulun tila **-sivulle.** Työnkulun tila -sivulla Sisäinen **tila -asetuksena** on Käynnistetty **ja** tietokuplassa näkyy teksti Ei voi lähettää **vastaanottajalle.**

Voit kiertää tämän ongelman määrittämällä työnkulun lähettämään sähköpostiviestejä [ylittämättä Exchange Online rajoja.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) Käytä esimerkiksi taukoa työnkulussa, lähetä sähköpostiviesti Microsoft 365-ryhmälle, jakeluryhmälle tai sähköpostia käyttävälle käyttöoikeusryhmälle tai lähetä viesti alle 200 vastaanottajalle kerrallaan.


Lisätietoja on seuraavassa [artikkelissa.](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)

## <a name="related-topics"></a>Aiheeseen liittyvät artikkelit
- [Luo Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ja Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 