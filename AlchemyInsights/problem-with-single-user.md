---
title: Ongelma yksittäisen käyttäjän kanssa
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
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429712"
---
# <a name="problem-with-single-user"></a>Ongelma yksittäisen käyttäjän kanssa

- Käyttäjää ei ehkä ole valmistettu, koska palvelussa ei ole vielä ollut mahdollisuutta arvioida käyttäjää. Tutustu valmistelun määrityssivun ohjeisiin sekä edistymispalkkiin. Jos lisätiedot-osassa määritetty tasainen tila on ennen käyttäjän luonti-, päivitys- tai poistamispäivää, se tarkoittaa, että käyttäjää ei ole vielä arvioitu. Tässä skenaariossa on parasta odottaa valmistelupalvelun valmistumista.

  - Huomaa, että palvelumme on tietoinen vain lähdejärjestelmän (Cloud HR) käyttäjälle muutoksista. Azure AD:n lähdejärjestelmässä on oltava kelvollinen muutos, jotta se voidaan tunnistaa ja se voidaan sitten työnkulun jälkeen käyttää Active Directorya.
- Valmistelupalvelu on arvioinut käyttäjän ja todennut, ettei sitä tule valmistella:
  - Jos olet määrittänyt määritepohjaisen rajaussuodattimen, varmista, että käyttäjä täyttää määrittämäsi ehdot.
  - Jos käyttäjät ovat jo kohdejärjestelmässä ja käyttäjän tila lähde- ja kohde vastineissa, emme tee mitään lisätoimia.
- Valmistelupalvelu yritti valmistella käyttäjää, ja se epäonnistui. Tutustu näissä tilanteissa valmistelulokien vianmääritys- ja suositukset-välilehteen:
  - Käyttäjän pakollinen määrite saattaa puuttua paikallisesta Active Directorysta tai Azure AD:stä. Esimerkiksi userPrincipalName- tai sAMAccountName-luontisäännöt eivät luo oikeaa arvoa.
  - Vastaava määrite (yleensä employeeId) ei ratkaise yksilöllistä käyttäjää paikalliselle Active Directorylle tai Azure AD:lle. Esimerkiksi kahdella käyttäjällä on sama työntekijätunnus AD:ssä, ja palvelu palauttaa virhekoodin, joka osoittaa saman lähdemerkinnän kohdemerkintöjen kaksoiskappaleet.

Jos haluat tarkastella yksittäisen käyttäjän ja ryhmän lokeja, tutustu tietyn käyttäjän ongelmaan tutustumalla [valmistelulokeja.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)
