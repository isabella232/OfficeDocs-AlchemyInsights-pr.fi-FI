---
title: Microsoft 365 Apps for Enterprisen käyttöönotto jaettua käyttöä varten RDS:ssä, päätepalvelimessa tai VDI:ssä
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
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200670"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Microsoft 365 Apps for Enterprisen käyttöönotto jaettua käyttöä varten RDS:ssä, päätepalvelimessa tai VDI:ssä

Microsoft 365 Apps for Enterprisen käyttöönotto etätyöpöytäpalveluja (RDS) käyttäen, aiemmin päätepalvelut:

- Sinulla on oltava Microsoft 365 For Business -palvelupaketti tai Office 365 -palvelupaketti, joka sisältää Microsoft 365 -sovellukset yrityksille, kuten Office 365 Enterprise E3 tai Enterprise E5.
   > [!NOTE]
   > Microsoft 365 Apps for Business- ja Microsoft 365 Business Standard -palvelupaketit eivät sisällä Microsoft 365 Apps for Enterprise -sovelluksia.
- Sinun on otettava käyttöön [jaetun tietokoneen aktivointi.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

> [!NOTE]
> Voit myös ladata ja suorittaa [Microsoftin tuki-](https://aka.ms/SaRA_OfficeSCA_M365Portal) ja palautusavustajan, jotta voit asentaa Microsoft 365 Apps for Enterprisen jaetussa tietokoneen aktivointitilassa.

Lisätietoja edellytyksistä, asennusohjeista ja mukautetuista asennuksista Officen käyttöönottotyökalun avulla on kohdassa [Microsoft 365 -sovellusten](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)käyttöönotto etätyöpöytäpalveluja käyttämällä.

Jaetun tietokoneen aktivointiin liittyvien virheiden korjaaminen:

- Katso [Microsoft 365 Apps for Enterprisen](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)jaetun tietokoneen aktivoinnin ongelmien vianmääritys.
- Katso [Palauta aktivointitila Microsoft 365 -yrityssovelluksille](https://go.microsoft.com/fwlink/?linkid=2109218).

Jos haluat asentaa Microsoft 365 Apps for Enterprisen RDS:lle Microsoft 365 -hallintakeskuksesta, joka käyttää oletusasennusasetuksia, toimi seuraavasti:

1. Tarkista, mikä tilaus sinulla on. [Ohjeet](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. Vaihda tarvittaessa toiseen tilaukseen. [Ohjeet](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Jos Office on jo asennettu RDS-palvelimeen muiden Microsoft-tilausten avulla, poista sen asennus. Voit esimerkiksi valita **Ohjauspaneelin Poista**  >  **ohjelman asennus**. Poista asennus [Microsoftin tuki-](https://aka.ms/SARA-OfficeUninstall-Alchemy) ja palautusavustajan avulla, jos sinulla on ongelmia.
4. Kirjaudu RDS-palvelimessa Microsoft 365 -hallintakeskukseen järjestelmänvalvojan tililläsi ja asenna [Microsoft 365 Apps for Enterprise.](https://portal.office.com/OLS/MySoftware.aspx)
5. Kun Office on asennettu, ***älä avaa tai kirjaudu*** sisään mihinkään Office-sovellukseen.
6. Ota RDS-palvelimessa käyttöön jaettu tietokoneaktivointi muokkaamalla rekisteriä seuraavasti:
   1. Napsauta näytön vasemmassa alakulmassa olevaa Windows-painiketta hiiren kakkospainikkeella ja valitse **Suorita.** Kirjoita Avaa-ruutuun **regedit** ja napsauta sitten **OK**.
   2. Valitse **Kyllä,** kun ohjelma pyytää sallimaan Rekisterieditorin tehdä muutoksia laitteeseesi.
   3. Lisää Rekisterieditorissa **SharedComputerLicensing-merkkijonoarvo,** jonka asetuksena on 1 kohdassa HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Kirjaudu RDS-palvelimessa käyttäjänä ja varmista, että Microsoft 365 Apps for Enterprise -sovellukset ovat käytössä  [jaetun tietokoneen aktivoinnissa.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)
