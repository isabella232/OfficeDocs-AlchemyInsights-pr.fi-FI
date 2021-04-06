---
title: Windowsin virtuaalityöpöydän ongelmien tunnistaminen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595628"
---
# <a name="identify-windows-virtual-desktop-issues"></a>Windowsin virtuaalityöpöydän ongelmien tunnistaminen

Windowsin virtuaalityöpöydän vianmääritys käyttää vain yhtä PowerShellin cmdlet-komentoa, mutta sisältää useita valinnaisia parametreja ongelmien rajaamista ja eristämista varten. Aloittaminen: 

1. Lataa ja tuo Windows Virtual Desktop PowerShell -moduuli. Lisätietoja on Windows [PowerShellin Windowsin virtuaalityöpöydän cmdlet-komennoissa.](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)

1. Kirjaudu tiliisi seuraavalla cmdlet-komennolla:
    
    Esimerkki: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**HUOMAUTUS:** Kaikissa PowerShellin kyselyissä on oltava joko -UserName- tai -ActivityID-parametrit. Lisätietoja valvontaominaisuuksista on kohdassa [Lokianalyysin käyttäminen vianmääritystoimintoa varten.](https://go.microsoft.com/fwlink/?linkid=2126847)

Jos haluat suodattaa diagnostiikkatoiminnot käyttäjän mukaan, suorita seuraava cmdlet-komento:

Esimerkki: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

Voit suorittaa vianmääritykseen suodattimien luettelon. Lisätietoja ongelmien selvittämiseksi on ohjeaiheessa Windowsin virtuaalityöpöydän ongelmien [tunnistaminen ja vianmääritys.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)

Lisätietoja yleisistä virheistä on kohdassa Yleiset [virheet senariot.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios)
