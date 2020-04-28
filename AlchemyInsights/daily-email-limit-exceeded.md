---
title: Päivittäinen sähköpostiraja ylitetty. Työnkulku on keskeytetty.
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
ms.openlocfilehash: 5a510f1137c7c49cd1de3d3fd2a470759e37ba1e
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908701"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Päivittäinen sähköpostiraja ylitetty. Työnkulku on keskeytetty.

Tämä virhe saattaa ilmetä seuraavissa tilanteissa:

- SharePoint Onlinessa on työnkulku, joka käyttää SharePoint 2010- tai SharePoint 2013 -työnkulkuympäristötyyppiä.
- Työnkulku on määritetty lähettämään mukautettu sähköpostiviesti yli 200 käyttäjälle kerrallaan, yli 10 000 vastaanottajalle päivässä tai yli 30 viestiä minuutissa.
- Kun suoritat työnkulun, sähköpostiviestiä ei lähetetä ja huomaat seuraavan ongelman:
    - Jos työnkulku on käytössä SharePoint 2013 -ympäristötyypin avulla, siirry **Työnkulun tila -sivulle.** Työnkulun tila -sivulla **Sisäinen tila** -asetuksena on **Aloitettu**ja tietokuplassa näkyy Ei voi **lähettää vastaanottajalle**.

Voit kiertää tämän ongelman määrittämällä työnkulun lähettämään sähköpostiviestejä ylittämättä [Exchange Online -lähettäjän rajoituksia.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) Käytä esimerkiksi keskeytystä työnkulussa, lähetä sähköpostiviesti Microsoft 365 -ryhmään, jakeluryhmään tai sähköpostia käyttävään suojausryhmään tai lähetä viesti alle 200 vastaanottajalle kerrallaan.


Lisätietoja on seuraavassa [artikkelissa](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Aiheeseen liittyvät artikkelit
- [Luo työnkulku](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ja Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 