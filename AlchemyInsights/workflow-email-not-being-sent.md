---
title: Työnkulun sähköpostia ei lähetetä
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
ms.openlocfilehash: 2caf8e0878da0049667d9a19f4488eaec4b9327fbf36be7d29dbf4b7a9c89158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072517"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Työnkulun sähköpostia ei lähetetä SharePoint luetteloa tai kirjastoa varten

1. Työnkulkujen sähköposteja ei lähetetä kaikille tai vain tietyille käyttäjille, tai saat virheilmoituksen Sähköpostiviestiä ei voi **lähettää.** Varmista, että sähköpostiviestissä on kelvollinen vastaanottaja .

    Tarkista, onko käyttäjä tämän **sivustokokoelman Kaikki** henkilöt -käyttöoikeusryhmässä (käyttäjätietojen luettelossa).  Suoran URL-osoitteen esimerkki: https:// <tenant> .sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId=0

    - Jos käyttäjää ei ole olemassa, varmista, että käyttäjä on kirjautunut sivulle. 
    - Jos käyttäjä on ulkoinen käyttäjä, varmista, että hänen kutsunsa on hyväksytty.
    - Jos käyttäjä on käyttöoikeusryhmässä, varmista, että sähköpostiosoite on oikea.
    - Jos käyttäjien sähköpostiosoitetta ei ole määritetty tässä kohdassa, luo käyttäjälle esimerkkiilmoitus, joka pakottaa tämän käyttäjätilin synkronoinnin käyttäjäprofiileista SharePoint tähän sivustokokoelmaan.
 
2. Työnkulkujen sähköpostit lähetetään sivustokokoelman järjestelmänvalvojille, mutta ei muille käyttäjille. Virhe http kielletty käyttäjälle **<span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail.**
 

    Katso [Käyttö estetty, kun lähetät sähköpostiviestin SharePoint ryhmälle.](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)

    Varmista myös, että **rajoitetun käytön käyttöoikeuden lukittu tila -sivustokokoelmaominaisuus** ei ole aktiivinen.


## <a name="related-topics"></a>Aiheeseen liittyvät artikkelit
Haluatko kokeilla Microsoft Flow online SharePoint ssa?
- [Luo Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ja Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


