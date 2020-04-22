---
title: Microsoft 365 Apps for enterprisen käyttöönotto jaettuun käyttöön RDS:ssä, Terminal Serverissä tai VDI:ssä
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: ddd44d40e9430ee31b8b734450dde0defef229d7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704702"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Microsoft 365 Apps for enterprisen käyttöönotto jaettuun käyttöön RDS:ssä, Terminal Serverissä tai VDI:ssä

Voit ottaa Microsoft 365 Apps for enterprise -sovelluksen käyttöön rds(Remote Desktop Services) -palvelun avulla, joka oli aiemmin nimetty päätepalveluksi:
- Sinulla on oltava Microsoft 365 For Business -palvelupaketti tai Office 365 -palvelupaketti, joka sisältää Microsoft 365 Apps for Enterprise -sovelluksen, kuten Office 365 Enterprise E3 tai Enterprise E5.
   > [!NOTE] 
   > Microsoft 365 Apps for Business- ja Microsoft 365 Business Premium Standard -palvelupaketit eivät sisällä Microsoft 365 Apps for enterprise -sovelluksia.
- [Jaettu tietokoneen aktivointi](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)on otettava käyttöön.

> [!NOTE]
> Voit myös ladata ja suorittaa [Microsoftin tuki- ja palautusavustajan,](https://aka.ms/SaRA_OfficeSCA_M365Portal) jos haluat asentaa Microsoft 365 Apps for enterprisen jaetun tietokoneen aktivointitilassa.

Lisätietoja mukautettujen asennusten edellytyksistä, asennusohjeista ja ohjeista Officen käyttöönottotyökalun avulla on ohjeaiheessa [Microsoft 365 Apps for enterprise -sovelluksen käyttöönotto etätyöpöytäpalveluiden avulla](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

Jaetun tietokoneen aktivointiin liittyvien virheiden korjaaminen:
- Lisätietoja [on ohjeaiheessa Microsoft 365 Apps for enterprise -sovelluksen jaetun tietokoneen aktivoinnin ongelmien vianmääritys](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Katso [Palauta aktivointitila Microsoft 365 -yrityssovelluksille](https://go.microsoft.com/fwlink/?linkid=2109218).

Jos haluat asentaa Microsoft 365 Apps for enterprisen RDS:ään Microsoft 365 -hallintakeskuksesta, ***joka käyttää asennuksen oletusasetuksia,*** toimi seuraavasti:

1.    Tarkista, mikä tilaus sinulla on. [Ohjeet](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.    Vaihda tarvittaessa toiseen tilaukseen. [Ohjeet](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.    Jos Office on jo asennettu RDS-palvelimeen muiden Microsoft-tilausten avulla, poista sen asennus. Esimerkiksi menemällä **Ohjauspaneeli** > **Poista ohjelma**. Poista asennus [Microsoftin tuki- ja palautusavustajan](https://aka.ms/SARA-OfficeUninstall-Alchemy) avulla, jos kohtaat ongelmia.
4.    Kirjaudu RDS-palvelimessa Microsoft 365 -hallintakeskukseen järjestelmänvalvojan tilillä ja [asenna Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).
5.    Kun Office on asennettu, ***älä avaa tai kirjaudu sisään*** mihinkään Office-sovellukseen.
6.    Ota jaettu tietokone aktivointi käyttöön RDS-palvelimessa muokkaamalla rekisteriä seuraavasti:
   1. Napsauta näytön vasemmassa alakulmassa olevaa Windows-painiketta hiiren kakkospainikkeella ja valitse **Suorita**. Kirjoita Avaa-ruutuun **regedit**ja valitse sitten **OK**.
   2. Valitse **Kyllä,** kun sinua kehotetaan sallimaan Rekisterieditorin tehdä muutoksia laitteeseesi.
   3. Lisää rekisterieditorissa **SharedComputerLicensing-merkkijono,** jonka asetus on 1 kohdassa HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Kirjaudu RDS-palvelimessa ***sisään loppukäyttäjänä*** ja [varmista, että jaetun tietokoneen aktivointi on otettu käyttöön Microsoft 365 Apps for enterprise -palvelussa.](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)

