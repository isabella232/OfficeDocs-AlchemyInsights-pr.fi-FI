---
title: Korjaa 0x8004de40-virhe OneDrivessa
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052034"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Korjaa 0x8004de40-virhe OneDrivessa

Jos näyttöön tulee virhe 0x8004de40 OneDrivessa:

- Käynnistä haavoittuvuuden sisältävät tieto kone uudelleen, kun olet muodostanut yhteyden Acitve-hakemisto toimi alueeseen.
- Jos uudelleenkäynnistys ei korjaa ongelmaa, avaa laitteen liitos ja liitä se uudelleen Azure ADISTA. 

**Huomautus**: sinun pitäisi olla yrityksen verkossa, kun suoritat näitä vaiheita. Älä tee näitä vaiheita, kun et pysty muodostamaan yhteyttä yrityksen infrastruktuuriin (esimerkiksi matkoilla). 

- Avaa laajennettu komento kehote. 
- Voit avata järjestelmänvalvojan oikeuksin suoritettavan komento kehotteen valitsemalla- **Käynnistä**, napsauttamalla hiiren kakkos painikkeella **komento kehote**-kohtaa ja valitsemalla sitten **Suorita järjestelmänvalvojana**.
- Kirjoita *dsregcmd/Leave* ja paina **ENTER**.
- Kun olet valmis, kirjoita *dsregcmd/Join* ja paina **ENTER**.
- Kun olet valmis, sulje komento kehote.
- Käynnistä tieto kone uudelleen ja Kirjaudu sisään OneDriveen.