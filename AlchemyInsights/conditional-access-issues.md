---
title: Ehdollisen käyttöoikeuden ongelmat
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 85cbd89e461f36a51eed816619fd132ea60dfdb0014eb850c7ec3f38d41e1ca2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069961"
---
# <a name="conditional-access-issues"></a>Ehdollisen käyttöoikeuden ongelmat

**Kirjautumisen vianmäärityksen ongelmien ratkaiseminen**

Kirjautumisen vianmäärityksen avulla voit selvittää nopeasti, mitä käyttäjän kirjautumisongelmat ovat tapahtuneet tai mikä on [vianmäärityksessä:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Käynnistä kirjautumisen vianmääritys.
1. Etsi analysoitava tapahtuma kirjoittamalla tiedot käyttäjästä, sovelluksesta, kirjautumisajasta, pyynnön tunnuksesta tai korrelaatiotunnuksesta.
1. Tarkista diagnostiikkatulokset, jotka näyttävät tiedot siitä, mitä on tapahtunut ja mitä voit tehdä muutosten tekoon (jos muutoksia tarvitaan).

**Kirjautumisen vianmääritys** 

1. Siirry Azure AD:n kirjautumissivulle.
1. Voit suodattaa kirjautumiset käyttäjän, aika-alueen, sovelluksen, tilan, asiakassovelluksen ja niin edelleen.
1. Valitse kirjautumistapahtuma ja tarkastele Ehdollinen käyttöoikeus -välilehteä, jotta näet, mitkä käytännöt on arvioitu.
1. Napsauta käytännön riviä, niin näet käytännön tiedot ja sen syyn.

**Työkalut ehdollisen käyttöoikeuden käytännön vianmääritykseen**

- Vain raportti -tilassa voit arvioida käytännön vaikuttamatta käyttäjiin.
- Entä jos -työkalun avulla voit simuloida kirjautumistapahtumia ja nähdä, mitä käytäntöjä sovelletaan.
- Insights raportointityökirja näyttää kunkin käytännön reaaliaikaisen vaikutuksen.

**Perusaikataulun suojauskäytännöt**

Perusaikataulun suojauskäytännöt on poistettu käytöstä. Niitä ei enää pakoteta, ja ne poistetaan pian Azure-portaalista. Suosittelemme, että otat [suojauksen oletusasetukset käyttöön.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)

Lisätietoja ehdollisesta käyttöoikeussta on kohdassa:

[Ehdollisen käyttöoikeuden parhaat käytännöt Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Ehdollisen käyttöoikeuden ehdot](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Ehdollisen käyttöoikeuden ohjausobjektit](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Sijainnit ehdollisessa käyttöoikeusssa](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
