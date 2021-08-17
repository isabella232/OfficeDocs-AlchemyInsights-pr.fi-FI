---
title: Officen asentaminen päätepalvelimeen – Ei käyttöomme
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 7e435df1515878ab4fe935ab8148daee29b8e3820095fc6e49db45de4c6279db
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055155"
---
# <a name="installing-office-on-a-terminal-server"></a>Office asentaminen päätepalvelimeen

Jos haluat ottaa Microsoft 365 -sovellukset suuryrityksille etätyöpöytäpalveluja (RDS) Windows palvelimessa, jonka nimi oli aiemmin Päätepalvelut:
  
- Sinulla on oltava Microsoft 365, joka sisältää Microsoft 365 -sovellukset suuryrityksille, kuten Office 365 Enterprise E3 tai Enterprise E5. Palvelupaketit Microsoft 365 -sovellukset yrityksille ja Microsoft 365 -sovellukset yrityksille Premium eivät sisällä Microsoft 365 -sovellukset suuryrityksille.

- Sinun on otettava käyttöön [jaetun tietokoneen aktivointi](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Jos haluat asentaa Microsoft 365 -sovellukset suuryrityksille RDS-Microsoft 365 -hallintakeskus, jossa käytetään ***oletusasennusasetuksia***, toimi seuraavasti.

> [!TIP]
> Voit myös ladata ja suorittaa [Microsoft tuki- ja palautusavustaja](https://aka.ms/SaRA_OfficeSCA_M365Portal) ja asentaa Microsoft 365 -sovellukset suuryrityksille jaetussa tietokoneen aktivointitilassa.
  
1. Tarkista Microsoft 365 tilaus. [Lisätietoja](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Vaihda tarvittaessa toiseen Microsoft 365 tilaukseen. [Lisätietoja](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Jos Office on jo asennettu RDS-palvelimeen käyttämällä muita Microsoft 365 tilauksia, poista sen asennus. Voit esimerkiksi valita Ohjauspaneelista Poista \> ohjelman asennus. Poista [asennus Microsoft tuki- ja palautusavustaja-ohjelman](https://aka.ms/SARA-OfficeUninstall-Alchemy) avulla, jos sinulla on ongelmia.

4. Kirjaudu RDS-palvelimessa Microsoft 365 -hallintakeskus järjestelmänvalvojan tilillä ja asenna [Microsoft 365 -sovellukset suuryrityksille.](https://portal.office.com/OLS/MySoftware.aspx)

5. Kun Office on asennettu, ***älä avaa*** tai kirjaudu sisään Office sovelluksiin.

6. Ota RDS-palvelimessa käyttöön jaetun tietokoneen aktivointi muokkaamalla rekisteriä seuraavasti:

1. Napsauta näytön Windows oikeassa alakulmassa olevaa Windows-painiketta hiiren kakkospainikkeella ja valitse Suorita. Kirjoita Avaa-ruutuun **regedit** ja valitse sitten OK.

2. Valitse pyydettäessä Kyllä, jos haluat, että Rekisterieditori voi tehdä muutoksia laitteeseesi.

3. Lisää Rekisterieditorissa **SharedComputerLicensing-merkkijonoarvo,** jonka asetus on 1 kohdassa HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Kirjaudu RDS-palvelimessa ***sisään käyttäjänä*** ja varmista, että jaetun tietokoneen aktivointi [on otettu käyttöön Microsoft 365 -sovellukset suuryrityksille.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)

Lisätietoja edellytyksistä, asennusohjeista ja mukautetuista asennuksista Office-käyttöönottotyökalun avulla on kohdassa [Microsoft 365 -sovellukset suuryrityksille käyttöönotto etätyöpöytäpalveluja käyttämällä.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)
  
Lisätietoja jaetun tietokoneen aktivointiin liittyvien virheiden korjaamisesta on kohdassa Jaetun tietokoneen aktivointiongelmien [vianmääritys Microsoft 365 -sovellukset suuryrityksille.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
  