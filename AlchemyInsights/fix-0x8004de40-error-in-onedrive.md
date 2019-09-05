---
title: Korjaa 0x8004de40-virhe OneDrivessa
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755845"
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