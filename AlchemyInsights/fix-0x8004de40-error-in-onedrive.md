---
title: Korjaa 0x8004de40-virhe OneDrivessa
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716025"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Korjaa 0x8004de40-virhe OneDrivessa

Jos saat 0x8004de40-virheen OneDrivessa:

- Käynnistä haavoittuvuuden sisältävä tietokone uudelleen, kun se on yhteydessä Acitve Directory -toimialueeseen.
- Jos uudelleenkäynnistys ei korjaa ongelmaa, poista liittyminen ja liity laitteeseesi uudelleen Azure AD:stä. 

**Huomautus:** Sinun pitäisi olla yrityksen verkossa, kun suoritat näitä vaiheita. Älä tee näitä vaiheita, kun et pysty muodostamaan yhteyttä yrityksen infrastruktuuriin (esimerkiksi matkoilla). 

- Avaa laajennettu komentokehote. 
- Voit avata komentorivin valitsemalla - **Käynnistä**, napsauttamalla **komentoriviä**hiiren kakkospainikkeella ja valitsemalla sitten **Suorita järjestelmänvalvojana**.
- Kirjoita *dsregcmd /leave* ja paina **Enter**.
- Kun olet valmis, kirjoita *dsregcmd /join* ja paina **Enter**.
- Kun olet valmis, sulje komentokehote.
- Käynnistä tietokone uudelleen ja kirjaudu OneDriveen.