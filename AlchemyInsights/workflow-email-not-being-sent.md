---
title: Työnkulun sähköpostia ei lähetetä
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766130"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Työnkulun sähköpostia ei lähetetä SharePoint-luetteloon tai kirjastoon

1. Työnkulkujen sähköpostia ei lähetetä kaikille käyttäjille tai vain tietyille käyttäjille, tai näet virheen **Sähköpostiviestiä ei voi lähettää. Varmista, että sähköpostiviestissä on kelvollinen vastaanottaja**.

    Tarkista, onko käyttäjä kyseisen sivustokokoelman **Kaikki henkilöt -käyttöoikeusryhmässä** (käyttäjätietoluettelo).  Esimerkki suorasta<tenant>URL-osoitteesta: https:// .sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId=0 (jäsenyysryhmä)=0

    - Jos käyttäjää ei ole, varmista, että käyttäjä on kirjautunut sivulle. 
    - Jos se on ulkoinen käyttäjä, varmista, että kutsu on hyväksytty.
    - Jos käyttäjä on käyttöoikeusryhmässä, varmista, että sähköpostiosoite on oikein.
    - Jos käyttäjien sähköpostiosoitetta ei ole määritetty tässä, luo kyseiselle käyttäjälle esimerkkiilmoitus, joka pakottaa kyseisen käyttäjätilin synkronoinnin SharePointin käyttäjäprofiileista tähän sivustokokoelmaan.
 
2. Työnkulkujen sähköposti lähetetään sivustokokoelman järjestelmänvalvojille, mutta ei muille käyttäjille, ja virhe **HTTP Kielletty <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Lisätietoja [on ohjeaiheessa Käyttö estetty, kun lähetät sähköpostia SharePoint-ryhmään](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Varmista myös, että **rajoitetun käytön käyttäjän käyttöoikeuksien lukitustilan** sivustokokoelmaominaisuus ei ole aktiivinen.


## <a name="related-topics"></a>Aiheeseen liittyvät artikkelit
Haluatko kokeilla Microsoft Flow'ta SharePoint Onlinessa?
- [Luo työnkulku](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ja Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


