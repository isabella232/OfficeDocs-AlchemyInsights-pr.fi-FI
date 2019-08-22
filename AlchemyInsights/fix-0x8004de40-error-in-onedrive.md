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
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525056"
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