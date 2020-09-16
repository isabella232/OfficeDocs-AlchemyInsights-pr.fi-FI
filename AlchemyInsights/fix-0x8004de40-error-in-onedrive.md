---
title: Korjaa 0x8004de40-virhe OneDrivessa
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745127"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Korjaa 0x8004de40-virhe OneDrivessa

Jos näyttöön tulee 0x8004de40-virhe OneDrivessa:

- Käynnistä haavoittuvuuden sisältävä tieto kone uudelleen, kun se on yhdistetty Acitve-hakemisto domainiin.
- Jos uudelleenkäynnistys ei korjaa ongelmaa, Yhdistä laite Azure AD:stä ja liity siihen uudelleen. 

**Huomautus**: sinun pitäisi olla yritys verkossasi, kun suoritat näitä vaiheita. Älä suorita näitä vaiheita, jos et voi muodostaa yhteyttä yrityksen infrastruktuuriin (esimerkiksi matkoilla). 

- Avaa järjestelmänvalvojan oikeuksin suoritettava komento kehote. 
- Avaa järjestelmänvalvojan oikeuksin suoritettava komento kehote napsauttamalla- **Käynnistä**, napsauttamalla hiiren kakkos painikkeella **komento kehote**ja valitsemalla sitten **Suorita järjestelmänvalvojana**.
- Kirjoita *dsregcmd/Leave* ja paina **ENTER**-näppäintä.
- Kun olet valmis, kirjoita *dsregcmd/Join* ja paina **ENTER**-näppäintä.
- Kun olet valmis, sulje komento kehote.
- Käynnistä tieto kone uudelleen ja Kirjaudu sisään OneDriveen.