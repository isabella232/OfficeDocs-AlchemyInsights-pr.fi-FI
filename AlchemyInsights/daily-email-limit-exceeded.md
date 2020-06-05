---
title: Päivittäinen sähköpostiraja ylittyi. Työnkulku on keskeytetty.
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
ms.openlocfilehash: 701c4aef6bfc0c4a2c4570f6dd16dbe4f99efc44
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580330"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Päivittäinen sähköpostin rajoitus ylitetty. Työnkulku on keskeytetty.

Tämä virhe voidaan saada seuraavissa tilanteissa:

- SharePoint Onlinessa on työnkulku, joka käyttää SharePoint 2010: n tai SharePoint 2013:n työnkulkuympäristötyyppiä.
- Työnkulku on määritetty lähettämään mukautettu sähköpostiviesti yli 200 käyttäjälle kerrallaan, yli 10 000 vastaanottajaa päivässä tai yli 30 viestiä minuutissa.
- Kun suoritat työnkulun, sähköpostiviestiä ei lähetetä, ja huomaat seuraavan toiminnan:
    - Jos työnkulku käyttää SharePoint 2013 -ympäristötyyppiä, siirry **Työnkulun tila -sivulle.** Työnkulun tila -sivulla **Sisäinen tila** -asetuksena on **Aloitettu**ja tietoselitteen näytössä Ei voi **lähettää vastaanottajalle**.

Voit kiertää tämän ongelman määrittämällä työnkulun lähettämään sähköpostiviestejä ylittämättä [Exchange Onlinen lähettäjän rajoituksia](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Käytä esimerkiksi työnkulun taukoa, lähetä sähköposti Microsoft 365 -ryhmään, jakeluryhmään tai sähköpostia käyttävään suojausryhmään tai lähetä viesti alle 200 vastaanottajalle kerrallaan.


Lisätietoja on seuraavassa [artikkelissa](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Aiheeseen liittyvät artikkelit
- [Luo työnkulku](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ja Työnkulku](https://flow.microsoft.com/blog/sharepoint-and-flow/) 