---
title: Työn kulun Sähkö posti viestiä ei lähetetä
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748986"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Työn kulun Sähkö posti viestiä ei lähetetä SharePoint-luettelolle tai-kirjastolle

1. Työn kulkujen Sähkö posti viestejä ei lähetetä kaikille käyttäjille tai vain tietyille käyttäjille, tai näet virhe ilmoituksen, **jonka mukaan Sähkö posti viestiä ei voi lähettää. Varmista, että sähkö posti viestissä on kelvollinen vastaanottaja**.

    Tarkista, onko käyttäjä olemassa kyseisen sivustokokoelman **Kaikki henkilöt** -käyttö oikeudet-ryhmässä (käyttäjä tiedot-luettelossa).  Esimerkki suora URL-osoitteesta: https:// <tenant> . SharePoint.com/sites/ <sitename> /_layouts/15/People.aspx? MembershipGroupId = 0

    - Jos käyttäjää ei ole olemassa, varmista, että käyttäjä on kirjautunut sivulle. 
    - Jos kyseessä on ulkoinen käyttäjä, varmista, että hänen kutsunsa on hyväksytty.
    - Jos käyttäjä on olemassa käyttö oikeudet-ryhmässä, varmista, että sähkö posti osoite on oikein.
    - Jos käyttäjien Sähkö posti osoitetta ei ole annettu tässä, luo kyseiselle käyttäjälle esimerkki ilmoitus, joka pakottaa kyseisen käyttäjä tilin synkronoinnin SharePointin käyttäjä profiileista tähän sivustokokoelmaan.
 
2. Työn kulkujen Sähkö posti viestit lähetetään sivustokokoelman järjestelmänvalvojille, mutta ei muille käyttäjille, ja Katso http-virhe ** <span>https:</span>//_vti_bin/Client.xvc.SP.Utilities.Utility.sendemail**.
 

    Katso [käyttö estetty, kun lähetät sähkö postia SharePoint-ryhmälle](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Varmista myös, että **rajoitetun käytön käyttö oikeuksien lukitus tilan** sivustokokoelman ominaisuus ei ole aktiivinen.


## <a name="related-topics"></a>Aiheeseen liittyvät artikkelit
Haluatko kokeilla Microsoft Flow'ta SharePoint Onlinessa?
- [Työn kulun luominen](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ja Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


