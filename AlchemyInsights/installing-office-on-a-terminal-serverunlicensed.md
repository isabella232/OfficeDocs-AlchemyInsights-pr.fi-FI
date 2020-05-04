---
title: Officen asentaminen päätepalvelimeen - Käyttöoikeudeton
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 6e952513679c9ac66f8de2b43d6d243cf17ff789
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010611"
---
# <a name="installing-office-on-a-terminal-server"></a>Officen asentaminen päätepalvelimeen

Microsoft 365 Apps for enterprisen käyttöönotto Windows Serverissä etätyöpöytäpalveluiden (RDS) avulla, aiemmin päätepalvelut:
  
- Sinulla on oltava Microsoft 365 -tilaus, joka sisältää Microsoft 365 Apps for Enterprise -sovelluksen, kuten Office 365 Enterprise E3 tai Enterprise E5. Microsoft 365 Apps for Business- ja Microsoft 365 Apps for Business Premium -palvelupaketit eivät sisällä Microsoft 365 Apps for enterprise -palvelupaketteja.

- Sinun on otettava [käyttöön jaetun tietokoneen aktivointi](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Jos haluat asentaa Microsoft 365 Apps for enterprisen RDS:ään Microsoft 365 -hallintakeskuksesta, ***joka käyttää asennuksen oletusasetuksia,*** toimi seuraavasti.

> [!TIP]
> Voit myös ladata ja suorittaa [Microsoftin tuki- ja palautusavustajan,](https://aka.ms/SaRA_OfficeSCA_M365Portal) jos haluat asentaa Microsoft 365 Apps for enterprisen jaetun tietokoneen aktivointitilassa.
  
1. Tarkista, mitä Microsoft 365 -tilausta sinulla on. [Lue lisää](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Vaihda tarvittaessa toiseen Microsoft 365 -tilaukseen. [Lue lisää](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Jos Office on jo asennettu RDS-palvelimeen muiden Microsoft 365 -tilausten avulla, poista sen asennus. Esimerkiksi menemällä Ohjauspaneeli \> Poista ohjelma. Poista asennus [Microsoftin tuki- ja palautusavustajan](https://aka.ms/SARA-OfficeUninstall-Alchemy) avulla, jos kohtaat ongelmia.

4. Kirjaudu RDS-palvelimessa Microsoft 365 -hallintakeskukseen järjestelmänvalvojan tilillä ja [asenna Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).

5. Kun Office on asennettu, ***älä avaa tai kirjaudu sisään*** mihinkään Office-sovellukseen.

6. Ota jaettu tietokone aktivointi käyttöön RDS-palvelimessa muokkaamalla rekisteriä seuraavasti:

1. Napsauta näytön vasemmassa alakulmassa olevaa Windows-painiketta hiiren kakkospainikkeella ja valitse Suorita. Kirjoita Avaa-ruutuun **regedit**ja valitse sitten OK.

2. Valitse Kyllä, kun sinua kehotetaan sallimaan Rekisterieditorin tehdä muutoksia laitteeseesi.

3. Lisää rekisterieditorissa **SharedComputerLicensing-merkkijono,** jonka asetus on 1 kohdassa HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Kirjaudu RDS-palvelimessa ***sisään loppukäyttäjänä*** ja [varmista, että jaetun tietokoneen aktivointi on otettu käyttöön Microsoft 365 Apps for enterprise -palvelussa.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)

Lisätietoja edellytyksistä, asennusohjeista ja mukautettujen asennusten ohjeista Officen käyttöönottotyökalun avulla on ohjeaiheessa [Microsoft 365 Apps for enterprise -sovelluksen käyttöönotto etätyöpöytäpalveluiden avulla](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Lisätietoja jaetun tietokoneen aktivointiin liittyvien virheiden korjaamisesta on [ohjeaiheessa Microsoft 365 Apps for enterprise -sovelluksen jaetun tietokoneen aktivoinnin ongelmien vianmääritys](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  