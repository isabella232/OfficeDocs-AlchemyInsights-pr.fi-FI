---
title: Kohteita ei voi poistaa SharePointissa tai OneDrivessa
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
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511973"
---
# <a name="unable-to-delete-items"></a>Kohteita ei voi poistaa

Säilytyskäytännöt voivat aiheuttaa tämän, sinun on joko poistettava käytöstä tai suljettava pois vastaava pito, joka aiheuttaa tämän ongelman. Kun säilytyskäytäntö tai pito on poistettu, muutoksen voimaantulo voi kestää jopa 24 tuntia. Varmista, että kohteessa ei ole [säilytyskäytäntöasetuksia.](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

Sivusto on saattanut ylittää tallennusrajan, suurentaa [sivuston kiintiötä](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) ja poistaa kohteen.

Varmista, että kohdetta ei ole [kuitattu ulos](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) toiselle käyttäjälle.

Lopuksi järjestelmänvalvojat voivat käyttää [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) -toimintoa, joka sisältää PowerShell-komentojen kirjaston, jonka avulla voit suorittaa monimutkaisia hallintatoimintoja, kuten pakottaa itsepintaisten kohteiden poistamisen.
- [Poista PNP-tiedosto](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Poista PNP-kansio](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Poista PNP-luettelokohde](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Poista PNP-luettelo](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [PNP-kentän poistaminen (sarake)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)