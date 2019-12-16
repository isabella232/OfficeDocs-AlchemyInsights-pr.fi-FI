---
title: Työn kulun sähkö postia ei lähetetä
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049370"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Työn kulun sähkö postia ei lähetetä SharePoint-luetteloon tai-kirjastoon

1. Työn kulkujen sähkö postia ei lähetetä kaikille käyttäjille tai vain tietyille käyttäjille, tai näkyviin tulee virhe, **jonka mukaan Sähkö posti viestiä ei voi lähettää. Varmista, että sähkö posti viestissä on kelvollinen vastaanottaja**.

    Tarkista, onko käyttäjä olemassa kyseisen sivustokokoelman **Kaikki henkilöt** -käyttö oikeudet-ryhmässä (käyttäjä tiedot-luettelossa).  Näyte suora URL-osoite<tenant>: https://<sitename>. SharePoint.com/sites//_layouts/15/People.aspx? MembershipGroupId = 0

    - Jos käyttäjää ei ole, varmista, että käyttäjä on kirjautuneena sivulle. 
    - Jos kyseessä on ulkoinen käyttäjä, varmista, että heidän kutsunsa on hyväksytty.
    - Jos käyttäjä on olemassa käyttö oikeudet-ryhmässä, varmista, että sähkö posti osoite on oikein.
    - Jos käyttäjien Sähkö posti osoitetta ei ole määritetty tässä, luo kyseiselle käyttäjälle näyte hälytys, joka pakottaa kyseisen käyttäjä tilin synkronoinnin SharePoint-käyttäjä profiileista tähän sivustokokoelmaan.
 
2. Työn kuluista lähetetyt Sähkö posti viestit lähetetään sivustokokoelman järjestelmänvalvojille, mutta ei muille käyttäjille, ja http-protokollaa ei ole **kielletty <span>https:/URL/</span>_vti_bin/Client.xvc.SP.Utilities.Utility.sendemail**.
 

    Katso [käyttö estetty, kun lähetät sähkö postia SharePoint-ryhmälle](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Varmista myös, että **rajoitetun käytön käyttö oikeuden lukitus tilan** sivustokokoelman ominaisuus ei ole aktiivinen.


## <a name="related-topics"></a>Aiheeseen liittyvät artikkelit
Haluatko kokeilla Microsoft Flow'ta SharePoint Onlinessa?
- [Luo työn kulku](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ja Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


