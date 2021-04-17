---
title: Olemassa olevan näytön vianmääritys
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824576"
---
# <a name="troubleshoot-an-existing-monitor"></a>Olemassa olevan näytön vianmääritys

Kokeile näitä ratkaisuja näytön vianmääritykseen. 

**Päivitä näyttösi näyttö:**

Paina samanaikaisesti seuraavia näppäimiä: Windows-näppäin + Ctrl + Vaihto + B. Tämä päivittää tietoliikenteen grafiikkaohjaimen kanssa. Näytöt vilkkuvat hetkellisesti ja palaavat muutaman sekunnin kuluttua.

**Monitorin laitteiston vianmääritys:**

1. Irrota kaapeli, joka yhdistää tietokoneen näyttöön, ja kytke se takaisin sisään.
2. Irrota kaikki muut kuin tärkeät laitteet tietokoneesta (kuten sovittimet tai telakalla).

**Jos olet hiljattain asentanut tietokoneeseen päivityksen, voit ottaa näyttöohjaimen takaisin näkyviin:**

1. Valitse **Käynnistä**, kirjoita **laitehallinta** ja **valitse tuloksista** Laitehallinta.
2. Laajenna **Näyttösovittimet-osa,** napsauta näyttösovitinta hiiren kakkospainikkeella ja valitse **Ominaisuudet**.
3. Siirry **Ohjain-välilehteen** ja valitse **Roll Back Driver (Takaisinohjain).** <br>
Huomautus: Jos tämä ei ole käytettävissä tai se  näkyy harmaana, siirry seuraavaan vaiheeseen valitsemalla alla olevista vaihtoehdoista Ei.
4. Tietokone on ehkä käynnistettävä uudelleen, ennen kuin muutokset tulevat voimaan.

**Poista näyttöohjain ja asenna se uudelleen:**

1. Valitse **Käynnistä**, kirjoita **laitehallinta** ja **valitse tuloksista** Laitehallinta.
2. Laajenna **Näyttösovittimet-osa,** napsauta näyttösovitinta hiiren kakkospainikkeella ja valitse **Poista laitteen asennus**. 
3. Valitse kohdan Poista **tämän laitteen ohjainohjelmistot vieressä olevaa ruutua** ja valitse **Poista asennus**.<br>
Huomautus: Sinua saatetaan pyytää käynnistämään tietokone uudelleen tässä vaiheessa. Muista kirjoittaa loput ohjeet muistiin ennen uudelleenkäynnistystä.
4. Avaa Laitehallinta uudelleen.
5. Laajenna **Näyttösovittimet-osa,** napsauta näyttösovitinta hiiren kakkospainikkeella ja valitse **Päivitä ohjain**.
6. Valitse **Etsi ohjainohjelmisto automaattisesti ja** noudata asennusohjeita.