---
title: Kohteiden poistaminen SharePointista tai OneDrivesta ei onnistu
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571247"
---
# <a name="unable-to-delete-items"></a>Kohteiden poistaminen ei onnistu

Säilytys käytännöt voivat aiheuttaa tämän, sinun on joko poistettava tai suljettava pois kyseinen ongelma, joka aiheuttaa tämän ongelman. Kun säilytys käytäntö tai pito on poistettu, muutos tulee voimaan 24 tunnin kuluttua. Varmista, että nimikkeellä ei ole [säilytys käytäntö](https://docs.microsoft.com/office365/securitycompliance/retention-policies) asetuksia.

Sivusto on saattanut ylittää tallennus rajoituksen, kasvattaa [sivuston kiintiötä](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) ja poistaa kohteen.

Varmista, että kohde ei ole [kuitattu ulos](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) toiselle käyttäjälle.

Järjestelmänvalvojilla on myös käytössä [SharePoint-malleja ja käytäntöjä](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), jotka sisältävät PowerShell-komentoja, joiden avulla voit suorittaa monimutkaisia hallinta toimintoja, kuten pakottaa itsepäiset kohteet.
- [Poista PNP-tiedosto](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Poista PNP-kansio](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Poista PNP-luettelo kohde](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Poista PNP-luettelo](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Poista PNP-kenttä (sarake)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)