---
title: Puuttuvia sähköpostiviestejä karanteenissa
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: bd5a04fd5abad962b4e85e009a9232e1a93219c238c629506df5cfb034453df2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892044"
---
# <a name="missing-emails-in-quarantine"></a>Puuttuvia sähköpostiviestejä karanteenissa

Järjestelmänvalvojat [voivat tarkastella, vapauttaa tai poistaa näitä viestejä](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Valitse Microsoft 365 Defender -portaalissa <https://security.microsoft.com> Tarkista  \> **karanteeni**. Jos haluat siirtyä suoraan **Karanteeni-sivulle,** käytä <https://security.microsoft.com/quarantine> -  

Lisätietoja haun/suodattimen arvoista, joita voit käyttää, on kohdassa Karanteeniin asetettujen viestien ja tiedostojen [hallinta järjestelmänvalvojana EOP:ssä.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Cmdlet-komennot, joita käytetään karanteeniin asetettujen viestien ja tiedostojen tarkastelemiseen ja hallintaan, ovat seuraavat:

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Huomaa, että tämä cmdlet-komento on vain viesteille, ei tiedostoille, jotka ovat peräisin Lokero-, SharePoint-, OneDrive- tai Microsoft Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
