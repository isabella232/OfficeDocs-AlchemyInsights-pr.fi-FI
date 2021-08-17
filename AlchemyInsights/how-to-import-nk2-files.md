---
title: how-to-import-nk2-files
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: f2b034926ec165b819119b5c4e060f10022d6017ec5dba8794d18ee3e96c709a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54043203"
---
# <a name="how-to-import-nk2-files"></a>.nk2-tiedostojen tuominen 

Kun käynnistät Microsoft Outlook 2013-, Outlook 2016-, Outlook 2019- tai Outlook for Microsoft 365-tiedoston ensimmäistä kertaa, kutsumanimivälimuisti (tallennettu *profiilinimi*.nk2-tiedostoon) tuodaan piilotettuun viestiin oletusviestisäilössä.

Jos haluat tuoda .nk2-tiedostoja Outlook 2013-, Outlook 2016-, Outlook 2019- tai Outlook for Microsoft 365-versioon, varmista, että .nk2-tiedosto on seuraavassa kansiossa: %appdata%\Microsoft\Outlook

**Huomautus:**.nk2-tiedostolla on oltava sama nimi kuin nykyisellä Outlook 2013- tai Outlook 2016 profiilillasi. Profiilin nimi on oletusarvoisesti "Outlook". Voit tarkistaa profiilin nimen seuraavasti: 
1. Napsauta **Käynnistä**-painiketta ja valitse **Ohjauspaneeli**.
2. Kaksoisnapsauta **Sähköposti-kohtaa.**
3. Valitse Sähköpostiasetukset-valintaikkunassa **Näytä profiilit**.
4. Valitse **Käynnistä** > **Suorita**.
5. Kirjoita **Avaa-ruutuun** outlook.exe */importnk2* ja valitse sitten **OK.** 

Kun olet tuonut .nk2-tiedoston, tiedoston sisältö yhdistetään postilaatikkoosi tallennettuun olemassa olevaan lempinimivälimuistiin.

**Huomautus:**.nk2-tiedoston tiedostotunniste on .old, kun seuraavan kerran käynnistät Outlook 2013-, Outlook 2016-, Outlook 2019- tai Outlook for Microsoft 365. Jos haluat tuoda .nk2-tiedoston uudelleen, poista ensin .old-tiedostotunniste.

Lisätietoja on kohdassa Automaattisen [täydennysluettelon tuominen tai kopioiminen toiseen tietokoneeseen.](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%)