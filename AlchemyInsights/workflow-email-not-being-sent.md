---
title: Työnkulun sähköposti ei lähetetä
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 783bf0a5721aa5db7088432c71e06cac6dc90513
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059601"
---
# <a name="workflow-email-is-not-being-sent"></a>Työnkulun sähköposti ei lähetetä

1. Kaikki käyttäjät tai vain tietyille käyttäjille ei lähetetä sähköposti-työnkulkuja tai nähdä virhe **sähköpostiviestiä ei voi lähettää. Varmista, että sähköpostiviestillä on kelvollinen vastaanottaja**.

Tarkista, onko käyttäjä ole **Kaikkien henkilöiden** oikeudet ryhmässä (käyttäjätietoluetteloon) kyseisen sivustokokoelman.  Näyte suoraan URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0

- Jos käyttäjä ei ole, varmista, että käyttäjä on kirjautunut sivulle. 
- Jos kyseessä on ulkoinen käyttäjä, varmista, että niiden kutsu on hyväksytty.
- Jos käyttäjä ole ryhmän käyttöoikeudet, varmista, että sähköpostiosoite on oikein.
- Jos käyttäjät sähköpostiosoitetta ei ole määritetty tässä, Luo malli-ilmoitus, joka pakottaa käyttäjätilin synkronointi käyttäjän profiilit SharePoint-sivustokokoelman käyttäjälle.
 
2. Työnkulut-sähköposti lähetetään sivustokokoelman järjestelmänvalvojat, mutta ei muiden käyttäjien ja tulla seuraava virhe **kiellettyä HTTP <spam> <spam> ** <spam> <spam>.
 

On [Estetty, kun lähetetty sähköpostiviesti on ryhmitelty](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).

Tarkista myös sivustokokoelman ominaisuuden **käyttöoikeus on rajoitettu käyttöoikeus lockdown tilassa** ei ole aktiivinen.

## <a name="related-topics"></a>Aiheeseen liittyvät artikkelit
- [Luo työnkulku](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint- ja](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


