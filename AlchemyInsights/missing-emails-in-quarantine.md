---
title: Puuttuvat sähköpostit karanteenissa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569228"
---
# <a name="missing-emails-in-quarantine"></a>Puuttuvat sähköpostit karanteenissa"

Järjestelmänvalvojat voivat [tarkastella, vapauttaa tai poistaa näitä viestejä.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Voit avata & Yhteensopivuuskeskuksen siirtymällä kohtaan [https://protection.office.com](https://protection.office.com/) . Voit avata Karanteeni-sivun suoraan siirtymällä kohtaan [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Voit tehdä hakuja seuraavilla arvoilla:  

- **Sanoman tunnus**: Sanoman yleinen yksilöllinen tunnus. Jos valitset viestin luettelosta, **Viestin tunnus -arvo** näkyy näkyviin tulevassa Tiedot-pikaikkunaruudussa. **Details** Järjestelmänvalvojat voivat etsiä viestejä ja niitä vastaavia message id -arvoja [viestien jäljityksen](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) avulla.
- **Lähettäjän sähköpostiosoite**: Yhden lähettäjän sähköpostiosoite.
- **Vastaanottajan sähköpostiosoite**: Yksittäisen vastaanottajan sähköpostiosoite.
- **Aihe**: Käytä viestin koko aihetta. Hakuun ei ole merkitystä.

Kun olet syöttänyt hakuehdot, suodata tulokset valitsemalla ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Päivitä-painike Päivitä.**  

Karanteenissa olevien viestien ja tiedostojen tarkastelemiseen ja hallintaan käytettävät cmdlet-komennot ovat seuraavat:
- [Poista-Quarantine-läävä](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Vienti-Karanteeni-lässä](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-Quarantine-läävä](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Huomaa, että tämä cmdlet-komento on tarkoitettu vain viesteille, ei ATP:n haittaohjelmille SharePoint Onlinelle, OneDrive for Businessille tai Teamsille.
- [Julkaisu-Quarantine-lässä](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)