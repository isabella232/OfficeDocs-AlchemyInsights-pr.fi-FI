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
ms.openlocfilehash: 12490df735ca8c524058404df92db79c6c5682fe2ecafe2b42baed70fa3ab142
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971336"
---
# <a name="user-provisioning"></a>Käyttäjien valmistelu

- Voit valmistella [käyttäjän tarvittaessa ja](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) saada yksityiskohtaiset diagnostiikkatiedot vaiheista.
- Lisätietoja käyttäjien ja ryhmien valmistelussa kohtaamistasi ongelmista on vianmääritysoppaassa Ei käyttäjiä [valmistellaan.](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)
- Jos huomaat, että käyttäjiä ei valmistella, katso kohta Valmistelulokit [(esikatselu)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) Azure Active Directory (AD). Etsi lokimerkintöjä, jotka liittyvät tiettyyn käyttäjään.
- Käynnistä valmistelu uudelleen säännöllisin väliajoin, jotta kaikki käyttäjät, jotka eivät ole jääneet edellisellä valmistelujaksolla, saavat ne uudelleen käyttöön.
- Käyttäjää/ryhmää ei ole ehkä valmistettu, koska palvelussamme ei ole vielä ollut mahdollisuutta arvioida käyttäjää. Tutustu valmistelun määrityksen sivun ohjeisiin sekä edistymispalkkiin. Jos lisätiedoissa määritetty tasainen tila on ennen päivämäärää, jolloin käyttäjä luotiin/ päivitettiin tai poistettiin, se tarkoittaa, että käyttäjää ei ole vielä arvioitu. Tässä skenaariossa on parasta odottaa valmistelupalvelun valmistumista. Jos vakaa tila on saavutettu, suosittelemme käynnistämään käyttöliittymän uudelleen Azure-portaalissa.
  - Huomaa, että palvelumme on tietoinen vain lähdejärjestelmän käyttäjään tai ryhmään (Azure Active Directory). Jos käyttäjä tai ryhmä poistetaan suoraan sovelluksesta (esimerkiksi ServiceNow), emme ole tietoisia muutoksista, eikä sitä voi enää takaisin käyttää lähdejärjestelmän käyttäjän tilan perusteella. Tässä skenaariossa on parasta palata takaisin suoraan kohdesovelluksessa.
- Palvelumme arvioi käyttäjän/ryhmän ja määrittää, ettei sitä pidä valmistella:
  - Jos olet määrittänyt laajuuden määritetyille käyttäjille ja ryhmille, tarkista, onko käyttäjä/ryhmä määritetty sovellukselle.
  - Jos käyttäjä/ryhmä on määritetty sovellukseen, varmista, että häntä ei ole määritetty oletuskäyttörooliin. Tätä roolia ei voi käyttää valmisteluun.
  - Jos olet määrittänyt määritepohjaisen suodatuksen, varmista, että käyttäjä täyttää määrittämäsi ehdot.
  - Jos käyttäjiä on jo kohdejärjestelmässä ja käyttäjän tila lähde- ja kohdesyssä, emme tee mitään lisätoimia.
- Palvelumme yritti valmistella käyttäjää, ja se epäonnistui. Tutustu näiden skenaarioiden vianmääritys- ja suositukset-välilehteen valmistelulokeja varten:
  - Käyttäjän pakollinen määrite saattaa puuttua Azure Active Directory tai se ei vastaa kolmannen osapuolen sovelluksen edellyttämää muotoa. Käyttäjän Maa-määritteen asetuksena voi olla esimerkiksi Yhdysvallat, kun sen pitäisi olla Yhdysvallat.
  - Määrite on viitemäärite, jota ei vielä ole kohdesovelluksessa. Viitemäärite on määrite, joka osoittaa toiseen objektiin, esimerkiksi ryhmään kuuluu käyttäjä. Käyttäjän tunnus olisi ryhmän jäsenmääritteellä, mutta se voidaan käsitellä vain, jos käyttäjäobjekti, jonka se osoittaa jo olemassa olevan.
