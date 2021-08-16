---
title: Kohteita ei voi poistaa SharePoint OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038514"
---
# <a name="unable-to-delete-items"></a>Kohteita ei voi poistaa

- Säilytyskäytännöt voivat aiheuttaa tämän, sinun on joko poistettava käytöstä tai poistettava pito, joka aiheuttaa tämän ongelman. Kun säilytyskäytäntö tai pito on poistettu, voi kestää jopa 24 tuntia, ennen kuin muutos tulee voimaan. Varmista, että kohteessa [ei ole säilytyskäytännön](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) asetuksia.

- Sivusto on ehkä ylittänyt tallennustilarajan, [suurentanut sivuston kiintiötä](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) ja poistanut kohteen.

- Varmista, että kohdetta ei [ole kuitattu ulos](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) toiselle käyttäjälle.

- Järjestelmänvalvojat voivat lisäksi käyttää SharePoint Patterns [and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), joka sisältää PowerShell-komentokirjaston, jonka avulla voit suorittaa monimutkaisia hallintatoimintoja, kuten pakottaa poistamaan tarpeettomia kohteita.
- [PNP-tiedoston poistaminen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Poista PNP-kansio](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Poista PNP-luettelokohde](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Poista PNP-luettelo](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Poista PNP-kenttä (sarake)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)