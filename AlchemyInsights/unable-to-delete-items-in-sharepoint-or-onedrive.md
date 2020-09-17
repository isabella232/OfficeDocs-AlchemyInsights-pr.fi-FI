---
title: Kohteita ei voi poistaa SharePointissa tai OneDrivessa
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
ms.openlocfilehash: fd12115214cc28b822cf7fa57fe9b86f76f7beb1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806108"
---
# <a name="unable-to-delete-items"></a>Kohteiden poistaminen ei onnistu

Säilytys käytännöt voivat aiheuttaa tämän ongelman, sinun on joko poistettava käytöstä tai jätettävä tämä ongelma huomiotta. Kun säilytys käytännön tai pito on poistettu, muutoksen voimaan jääminen voi kestää jopa 24 tuntia. Varmista, että kohteessa ei ole [säilytys käytännön](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) määritystä.

Sivuston tallennus tila on ehkä ylitetty, kasvata [sivuston kiintiötä](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) ja Poista kohde.

Varmista, ettei kohdetta ole [kuitattu ulos](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) toiselle käyttäjälle.

Lopuksi järjestelmänvalvojat voivat käyttää [SharePoint-malleja ja-käytäntöjä](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), jotka sisältävät PowerShell-komentoja, joiden avulla voit suorittaa monimutkaisia hallinta toimintoja, kuten pakottaa poistamaan itsepäisiä kohteita.
- [PNP-tiedoston poistaminen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [PNP-kansion poistaminen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [PNP-luettelon kohteen poistaminen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [PNP-luettelon poistaminen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [PNP-kentän (sarakkeen) poistaminen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)