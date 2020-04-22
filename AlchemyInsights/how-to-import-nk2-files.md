---
title: how-to-import-nk2-files miten-to-import-nk2-tiedostot
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: 83d30b2d62908db791f21ec5ed7fd5537e7a0944
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759329"
---
# <a name="how-to-import-nk2-files"></a>.nk2-tiedostojen tuominen 

Kun käynnistät Microsoft Outlook 2013:n, Outlook 2016:n, Outlook 2019:n tai Outlook for Microsoft 365:n ensimmäistä kertaa, lempinimivälimuisti (joka on tallennettu *profiilinimeen*.nk2-tiedostoon) tuodaan piilotettuun viestiin oletusviestisäilössä.

Jos haluat tuoda .nk2-tiedostoja Outlook 2013:iin, Outlook 2016:iin, Outlook 2019:n tai Outlook for Microsoft 365:n versioon, varmista, että .nk2-tiedosto on seuraavassa kansiossa: %appdata%\Microsoft\Outlook

**Huomautus**: .nk2-tiedostolla on oltava sama nimi kuin nykyisellä Outlook 2013- tai Outlook 2016 -profiilillasi. Profiilin nimi on oletusarvoisesti Outlook. Voit tarkistaa profiilin nimen seuraavasti: 
1. Napsauta **Käynnistä -painiketta**ja valitse sitten **Ohjauspaneeli**.
2. Kaksoisnapsauta Mail .double-click **Mail**.
3. Valitse Sähköpostin asetukset -valintaikkunassa **Näytä profiilit**.
4. Valitse **Aloita** > **suoritus**.
5. Kirjoita **Avaa-ruutuun** *outlook.exe /importnk2*ja valitse sitten **OK**. 

Kun olet tuonut .nk2-tiedoston, tiedoston sisältö yhdistetään postilaatikkoon tallennettuun lempinimivälimuistiin.

**Huomautus**: .nk2-tiedosto nimetään uudelleen .old-tiedostotunnisteella, kun seuraavan kerran käynnistät Outlook 2013:n, Outlook 2016:n, Outlook 2019:n tai Outlook for Microsoft 365:n. Jos haluat tuoda .nk2-tiedoston uudelleen, poista .old-tiedostotunniste ensin.

Lisätietoja on [ohjeaiheessa Automaattisen täydennyksen luettelon tuominen tai kopioiminen toiseen tietokoneeseen](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).