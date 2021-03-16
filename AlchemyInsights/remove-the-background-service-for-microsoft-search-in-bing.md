---
title: Microsoft Searchin taustapalvelun poistaminen Bingissä
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816198"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>Microsoft Searchin taustapalvelun poistaminen Bingissä

Voit poistaa Microsoft Searchin taustapalvelun Bingissä kokeilemalla seuraavia korjaustoimenpiteitä:

1. Voit palauttaa alkuperäiset hakukoneasetukset seuraavasti:

    a. Vaihda Käytä **Bingiä oletushakukoneena [-vaihtopainike pois](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) käytöstä.**

    b. [Siirry Microsoft 365 -hallintakeskukseen](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) ja poista asetus, joka vaikuttaa organisaatiosi kaikkiin käyttäjiin.

2. Voit poistaa taustapalvelun yksittäisestä laitteesta seuraavasti:

    a. Valitse **Ohjauspaneeli > ohjelmat > ja toiminnot -kohdassa.**

    b. Napsauta **Bingissä hiiren kakkospainikkeella Microsoft Searchia** asennettujen ohjelmien luettelossa ja valitse sitten **Poista asennus.**

3. Jos haluat poistaa taustapalvelun useista organisaation laitteista, kirjaudu sisään järjestelmänvalvojana ja suorita seuraava komento komentosarjassa: 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
