---
title: Käyttäjien valmistelu
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004348"
- "8428"
ms.openlocfilehash: bd415b2d44bccf0c2b3eccb4e38452498b748b3a
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481360"
---
# <a name="user-provisioning"></a>Käyttäjien valmistelu

- Voit valmistella [käyttäjän tarvittaessa -valmistelun](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) avulla ja saada yksityiskohtaiset diagnostiikkatiedot vaiheista.
- Lisätietoja käyttäjien ja ryhmien valmistelussa kohtaamistasi ongelmista on vianmääritysoppaassa Ei käyttäjiä [valmistella.](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)
- Jos huomaat, että käyttäjiä ei valmistella, tutustu Azure Active [Directoryn (AD)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) valmistelulokeja (esiversio) -artikkeliin. Hae lokimerkintöjä, jotka liittyvät tiettyyn käyttäjään.
- Käynnistä valmistelu uudelleen säännöllisin väliajoin, jotta kaikki käyttäjät, jotka jäivät vastaamatta edellisellä valmistelujaksolla.
- Käyttäjää tai ryhmää ei ole ehkä valmistettu, koska palvelussamme ei ole vielä ollut mahdollisuutta arvioida käyttäjää. Tutustu valmistelun määrityssivun ohjeisiin sekä edistymispalkkiin. Jos lisätiedot-osassa määritetty tasainen tila on ennen käyttäjän luonti-, päivitys- tai poistamispäivää, se tarkoittaa, että käyttäjää ei ole vielä arvioitu. Tässä skenaariossa on parasta odottaa valmistelupalvelun valmistumista. Jos tasainen tila on saavutettu, suosittelemme käynnistämään käyttöliittymän uudelleen Azure-portaalissa.
  - Huomaa, että palvelumme on tietoinen vain lähdejärjestelmän käyttäjän tai ryhmän muutoksista (Azure Active Directory). Jos käyttäjä tai ryhmä poistetaan suoraan sovelluksesta (esimerkiksi ServiceNow), emme ole tietoisia näistä muutoksista eikä niitä poisteta lähdejärjestelmän käyttäjän tilan perusteella. Tässä skenaariossa muutos on parasta ottaa takaisin suoraan kohdesovelluksessa.
- Palvelumme arvioi käyttäjän/ryhmän ja määritti, ettei sitä tule valmistella:
  - Jos olet määrittänyt laajuuden määritetyille käyttäjille ja ryhmille, tarkista, onko käyttäjä/ryhmä määritetty sovellukselle.
  - Jos käyttäjä/ryhmä on määritetty sovellukseen, varmista, että häntä ei ole määritetty oletuskäyttörooliin. Tätä roolia ei voi käyttää valmistelussa.
  - Jos olet määrittänyt määritepohjaisen rajaussuodattimen, varmista, että käyttäjä täyttää määrittämäsi ehdot.
  - Jos käyttäjät ovat jo kohdejärjestelmässä ja käyttäjän tila lähde- ja kohde vastineissa, emme tee mitään lisätoimia.
- Palvelumme yritti valmistella käyttäjää, ja se epäonnistui. Tutustu näissä tilanteissa valmistelulokien vianmääritys- ja suositukset-välilehteen:
  - Käyttäjän pakollinen määrite saattaa puuttua Azure Active Directorysta tai se ei vastaa kolmannen osapuolen sovelluksen edellyttämää muotoa. Käyttäjän Maa-määritteen asetuksena voi olla esimerkiksi Yhdysvallat, kun sen pitäisi olla Yhdysvallat.
  - Määrite on viitemäärite, jota ei ole vielä kohdesovelluksessa. Viitemäärite on määrite, joka osoittaa toiseen objektiin, esimerkiksi ryhmään kuuluu käyttäjä. Käyttäjän tunnus olisi ryhmän jäsenmääritteellä, mutta sitä voidaan käsitellä vain, jos sen jo viittaama käyttäjäobjekti on olemassa.
