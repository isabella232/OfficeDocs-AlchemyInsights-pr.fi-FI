---
title: Korjaa virhe 0x8004de40 OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133974"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Korjaa virhe 0x8004de40 OneDrive

Jos näyttöön tulee virhesanoma 0x8004de40 OneDrive kanssa:

- Uudelleenkäynnistystä tietokonetta yhdistettynä Acitve Directory-toimialueeseen.
- Jos uudelleenkäynnistys ei korjaa ongelmaa, eroa ja liittyä Azure AD: stä laitteeseen. 

**Huomautus**: näiden vaiheiden aikana on oltava yrityksen verkossa. Älä suorita nämä vaiheet, kun et pysty muodostamaan yhteyttä yrityksen infrastruktuurin (esimerkiksi matkoilla). 

- Avaa järjestelmänvalvojan oikeuksin suoritettava komentokehote. 
- Avaa järjestelmänvalvojan oikeuksin suoritettava komentokehote, napsauta - **Käynnistä-painiketta**hiiren kakkospainikkeella **Komentorivi**ja valitsemalla **Suorita järjestelmänvalvojana**.
- Kirjoita *dsregcmd /leave* ja paina **Enter**-näppäintä.
- Kun asennus on valmis, kirjoita *dsregcmd /join* ja paina **Enter**.
- Kun olet valmis, sulje komentokehote.
- Käynnistä tietokone uudelleen ja kirjaudu järjestelmään OneDrive.