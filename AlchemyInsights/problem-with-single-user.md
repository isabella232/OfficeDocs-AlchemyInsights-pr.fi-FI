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
ms.openlocfilehash: 8d8821cda94b2af244fa317707421f9d197b6052fb316789cd286ea8b4adf19e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960148"
---
# <a name="problem-with-single-user"></a>Ongelma yksittäisen käyttäjän kanssa

- Käyttäjää ei ehkä ole valmistettu, koska palvelu ei ole vielä löytänyt mahdollisuutta arvioida käyttäjää. Tutustu valmistelun määrityksen sivun ohjeisiin sekä edistymispalkkiin. Jos lisätiedoissa määritetty tasainen tila on ennen päivämäärää, jolloin käyttäjä luotiin/ päivitettiin tai poistettiin, se tarkoittaa, että käyttäjää ei ole vielä arvioitu. Tässä skenaariossa on parasta odottaa valmistelupalvelun valmistumista.

  - Huomaa, että palvelumme on tietoinen vain lähdejärjestelmän (Cloud HR) käyttäjään muutoksista. Azure AD:n lähdejärjestelmässä on oltava kelvollinen muutos, jotta se voidaan tunnistaa ja työnkulkua Active Directoryyn.
- Provisioning service evaluated the user and determined it should not be provisioned:
  - Jos olet määrittänyt määritepohjaisen suodatuksen, varmista, että käyttäjä täyttää määrittämäsi ehdot.
  - Jos käyttäjiä on jo kohdejärjestelmässä ja käyttäjän tila lähde- ja kohdesyssä, emme tee mitään lisätoimia.
- Valmistelupalvelu yritti valmistella käyttäjää, ja se epäonnistui. Tutustu näiden skenaarioiden vianmääritys- ja suositukset-välilehteen valmistelulokeja varten:
  - Käyttäjän pakollinen määrite saattaa puuttua paikallisesta Active Directorysta tai Azure AD:stä. Esimerkiksi userPrincipalName- tai sAMAccountName-luontisäännöt eivät luo oikeaa arvoa.
  - Vastaava määrite (yleensä employeeId) ei ratkaise yksilöllistä käyttäjää paikalliselle Active Directorylle tai Azure AD:lle. On esimerkiksi kaksi käyttäjää, joilla on sama employeeId AD:ssä, ja palvelu palauttaa virhekoodin, joka osoittaa samalle lähdemerkinnälle samat kohdemerkinnät.

Jos haluat tarkastella yksittäisen käyttäjän ja ryhmän lokeja, katso tietyn käyttäjän ongelmia koskevat [valmistelulokit.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)
