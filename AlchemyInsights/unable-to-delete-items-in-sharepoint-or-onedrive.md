---
title: Kohteiden poistaminen SharePointista tai OneDrivesta ei onnistu
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3cc168846999c6880b95edfaedb2df8cf6e843a6
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36748547"
---
# <a name="unable-to-delete-items"></a>Kohteiden poistaminen ei onnistu

Onko sinulla ongelmia SharePoint-kohteiden poistamisessa?

- Varmista aina, että sinulla on [tarvittavat oikeudet](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) kohteen poistamiseen tai että [sivustokokoelman järjestelmänvalvoja](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) yrittää poistaa kohteen.

- Varmista, että nimikkeellä ei ole [säilytys käytäntö](https://docs.microsoft.com/office365/securitycompliance/retention-policies) asetuksia.

- Varmista, että kohde ei ole [kuitattu ulos](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) toiselle käyttäjälle.

- Järjestelmänvalvojilla on myös käytössä [SharePoint-malleja ja käytäntöjä](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), jotka sisältävät PowerShell-komentoja, joiden avulla voit suorittaa monimutkaisia hallinta toimintoja, kuten pakottaa itsepäiset kohteet.
- [Poista PNP-tiedosto](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Poista PNP-kansio](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Poista PNP-luettelo kohde](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Poista PNP-luettelo](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Poista PNP-kenttä (sarake)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)