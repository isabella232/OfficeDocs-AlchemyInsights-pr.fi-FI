---
title: Ehdollisen käytön ongelmat
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
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014789"
---
# <a name="conditional-access-issues"></a>Ehdollisen käytön ongelmat

**Kirjautumisen vianmäärityksen ongelmien ratkaiseminen**

Kirjautumisen vianmäärityksen avulla voit selvittää nopeasti, mitä on tapahtunut tai diagnosoida käyttäjien [kirjautumisongelmia:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Käynnistä kirjautumisen vianmääritys.
1. Etsi analysoitava tapahtuma kirjoittamalla tiedot käyttäjästä, sovelluksesta, kirjautumisajasta, pyyntötunnuksesta tai korrelaatiotunnuksesta.
1. Tarkista diagnostiikkatulokset, jotka näyttävät, mitä on tapahtunut ja mitä voit tehdä muutosten tekoon (jos muutoksia tarvitaan).

**Kirjautumisen vianmääritysvaiheet** 

1. Siirry Azure AD:n kirjautumissivulle.
1. Voit suodattaa kirjautumiset käyttäjän, aika-alueen, sovelluksen, tilan, asiakassovelluksen ja niin edelleen.
1. Valitse kirjautumistapahtuma ja tarkastele Ehdollinen käyttöoikeus -välilehteä nähdäksesi, mitkä käytännöt on arvioitu.
1. Napsauta käytännön riviä, jotta näet käytännön tiedot ja ymmärrät, miksi sitä on käytetty.

**Työkalut ehdollisen käytön käytännön vianmääritykseen**

- Vain raportti -tilassa voit arvioida käytäntöä vaikuttamatta käyttäjiin.
- Entä jos -työkalun avulla voit jäljitellä kirjautumistapahtumia ja nähdä, mitä käytäntöjä sovelletaan.
- Insights- ja Reporting-työkirja näyttää kunkin käytännön reaaliaikaisen vaikutuksen.

**Perusaikataulun suojauskäytännöt**

Perusaikataulun suojauskäytännöt on poistettu käytöstä. Niitä ei enää pakoteta, ja ne poistetaan pian Azure-portaalista. Suosittelemme, että otat [suojauksen oletusasetukset käyttöön.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)

Lisätietoja ehdollisesta käyttöoikeussta on kohdassa:

[Ehdollisen käyttöoikeuden parhaat käytännöt Azure Active Directoryssa](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Ehdollisen käyttöoikeuden ehdot](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Ehdollisen käyttöoikeuden ohjausobjektit](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Sijainnit ehdollisessa käyttöomme](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
