---
title: Rds Microsoft 365 -sovellukset suuryrityksille päätepalvelimen tai VDI:n jaetun käytön käyttöönotto
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 55b86557ec205dde2c459d76e8e330d2a8271dbec723f079e119ebe409b41c3f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031475"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Rds Microsoft 365 -sovellukset suuryrityksille päätepalvelimen tai VDI:n jaetun käytön käyttöönotto

Jos haluat Microsoft 365 -sovellukset suuryrityksille etätyöpöytäpalveluja (RDS) käyttäen, joiden nimi oli aiemmin Päätepalvelut:

- Sinulla on oltava Microsoft 365 For Business -Office 365, joka sisältää Microsoft 365 -sovellukset suuryrityksille,, Office 365 Enterprise E3 tai Enterprise E5.
   > [!NOTE]
   > Palvelupaketit Microsoft 365 -sovellukset yrityksille ja Microsoft 365 Business Standard eivät sisällä Microsoft 365 -sovellukset suuryrityksille.
- Sinun on otettava käyttöön [jaetun tietokoneen aktivointi](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Voit myös ladata ja suorittaa [Microsoft tuki- ja palautusavustaja](https://aka.ms/SaRA_OfficeSCA_M365Portal) ja asentaa Microsoft 365 -sovellukset suuryrityksille jaetussa tietokoneen aktivointitilassa.

Lisätietoja mukautettujen asennusten edellytyksistä, asennusohjeista ja Office-käyttöönottotyökalun avulla on kohdassa Microsoft 365 -sovellukset suuryrityksille käyttöönotto [etätyöpöytäpalvelujen avulla.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)

Jaetun tietokoneen aktivointiin liittyvien virheiden korjaaminen:

- Katso [jaetun tietokoneen aktivointiongelmien vianmääritys Microsoft 365 -sovellukset suuryrityksille.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
- Katso [Palauta aktivointitila Microsoft 365 -yrityssovelluksille](https://go.microsoft.com/fwlink/?linkid=2109218).

Jos haluat asentaa Microsoft 365 -sovellukset suuryrityksille RDS-Microsoft 365 -hallintakeskus, joka käyttää ***oletusasennusasetuksia***, toimi seuraavasti:

1. Tarkista, mikä tilaus sinulla on. [Ohjeet](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. Vaihda tarvittaessa toiseen tilaukseen. [Ohjeet](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Jos Office RDS-palvelimeen käyttämällä muita Microsoft-tilauksia, poista sen asennus. Voit esimerkiksi valita **Ohjauspaneelista Poista**  >  **ohjelman asennus**. Poista [asennus Microsoft tuki- ja palautusavustaja-ohjelman](https://aka.ms/SARA-OfficeUninstall-Alchemy) avulla, jos sinulla on ongelmia.
4. Kirjaudu RDS-palvelimessa Microsoft 365 -hallintakeskus järjestelmänvalvojan tilillä ja asenna [Microsoft 365 -sovellukset suuryrityksille.](https://portal.office.com/OLS/MySoftware.aspx)
5. Kun Office on asennettu, ***älä avaa*** tai kirjaudu sisään Office sovelluksiin.
6. Ota RDS-palvelimessa käyttöön jaetun tietokoneen aktivointi muokkaamalla rekisteriä seuraavasti:
   1. Napsauta näytön Windows näytön vasemmassa alakulmassa olevaa Windows-painiketta hiiren kakkospainikkeella ja valitse **Suorita**. Kirjoita Avaa-ruutuun **regedit** ja napsauta sitten **OK**.
   2. Valitse **pyydettäessä** Kyllä, jos haluat, että Rekisterieditori voi tehdä muutoksia laitteeseesi.
   3. Lisää Rekisterieditorissa **SharedComputerLicensing-merkkijonoarvo,** jonka asetus on 1 kohdassa HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Kirjaudu RDS-palvelimessa ***sisään käyttäjänä*** ja varmista, että jaetun tietokoneen aktivointi [on otettu käyttöön Microsoft 365 -sovellukset suuryrityksille.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)
