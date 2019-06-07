---
title: Voi poistaa kohteita SharePoint-tai OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 82a19c8ea218834b71901e95747da0c99243893e
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757922"
---
# <a name="unable-to-delete-items"></a>Kohteiden poistaminen ei onnistu

Kohteiden poistaminen ongelmia?

- Varmista aina, että sinulla on [riittävät oikeudet](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) poistaa kohteen tai poistaa kohteen [Sivustokokoelman järjestelmänvalvoja](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) -yritys.

- Varmistaa, että ei ole [säilytyskäytäntö](https://docs.microsoft.com/office365/securitycompliance/retention-policies) asetukset kohteessa.

- Varmista kohde on [kuitattu ulos](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) toiselle käyttäjälle.

- Lisäksi järjestelmänvalvojat voivat käyttää [SharePoint-kuviot ja käytäntöjä](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) joka sisältää kirjaston PowerShellin komennot, joiden avulla voit tehdä monimutkaisia hallinnan toimintoja kuten pakottaa stubborn poistosta. 
- [PNP-tiedoston poistaminen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [PNP-kansion poistaminen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Poista luettelokohteen PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Poista PNP-luettelo](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Poista Plug and Play-kenttä (sarake)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)