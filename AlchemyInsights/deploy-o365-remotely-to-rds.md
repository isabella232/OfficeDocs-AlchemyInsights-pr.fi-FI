---
title: Microsoft 365 -sovellusten käyttöönotto jaettua käyttöä varten RDS:ssä, Terminal Serverissä tai VDI:ssä
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
ms.openlocfilehash: fe051cd1dac899dc9bb19d275c352ec6585b6a93
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507583"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Microsoft 365 -sovellusten käyttöönotto jaettua käyttöä varten RDS:ssä, Terminal Serverissä tai VDI:ssä

Microsoft 365 Apps for enterprise -sovellukset etätyöpöytäpalveluiden (RDS) avulla, jotka oli aiemmin nimetty päätepalveluilla:
- Sinulla on oltava Microsoft 365 For Business -palvelupaketti tai Office 365 -palvelupaketti, joka sisältää Microsoft 365 Apps for Enterprise -sovellukset, kuten Office 365 Enterprise E3:n tai Enterprise E5:n.
   > [!NOTE] 
   > Microsoft 365 -sovellukset yrityksille ja Microsoft 365 Business Premium Standard -palvelupaketit eivät sisällä Microsoft 365 Apps for enterprise -sovelluksia.
- [Jaetun tietokoneen aktivointi](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)on otettava käyttöön .

> [!NOTE]
> Voit myös ladata ja suorittaa [Microsoftin tuki- ja palautusavustajan](https://aka.ms/SaRA_OfficeSCA_M365Portal) ja asentaa Microsoft 365 Apps for enterprise -sovelluksen jaetun tietokoneen aktivointitilassa.

Lisätietoja mukautettujen asennusten edellytyksistä, asennusohjeista ja ohjeista Officen käyttöönottotyökalun avulla on [ohjeaiheessa Microsoft 365 -sovellusten käyttöönotto yrityksille etätyöpöytäpalveluiden avulla](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Voit korjata jaetun tietokoneen aktivointiin liittyvät virheet:
- Lisätietoja [on ohjeaiheessa Microsoft 365 Apps for enterprise -sovellusten jaetun tietokoneen aktivointiin liittyvien ongelmien vianmääritys](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Katso [Palauta aktivointitila Microsoft 365 -yrityssovelluksille](https://go.microsoft.com/fwlink/?linkid=2109218).

Jos haluat asentaa Microsoft 365 Apps for enterprise -sovellukset RDS:ään Microsoft 365 -hallintakeskuksesta, ***joka käyttää oletusasennusasetuksia,*** toimi seuraavasti:

1.    Tarkista, mikä tilaus sinulla on. [Ohjeet](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2.    Vaihda tarvittaessa toiseen tilaukseen. [Ohjeet](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3.    Jos Office on jo asennettu RDS-palvelimeen millä tahansa muulla Microsoft-tilauksella, poista sen asennus. Jos esimerkiksi siirryt **Ohjauspaneeliin**  >  **Poista ohjelman asennus**. Poista asennus [Microsoftin tuki- ja palautusavustajan](https://aka.ms/SARA-OfficeUninstall-Alchemy) avulla, jos sinulla on ongelmia.
4.    Kirjaudu RDS-palvelimessa Microsoft 365 -hallintakeskukseen järjestelmänvalvojan tilillä ja [asenna Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).
5.    Kun Office on asennettu, ***älä avaa tai kirjaudu mihinkään*** Office-sovellukseen.
6.    Ota jaetun tietokoneen aktivointi käyttöön RDS-palvelimessa muokkaamalla rekisteriä seuraavasti:
   1. Napsauta näytön vasemmassa alakulmassa olevaa Windows-painiketta hiiren kakkospainikkeella ja valitse **Suorita**. Kirjoita Avaa-ruutuun **regedit**ja valitse sitten **OK**.
   2. Valitse **Kyllä,** kun sinua kehotetaan antamaan Rekisterieditorin tehdä muutoksia laitteeseesi.
   3. Lisää SharedComputerLicensing-merkkijonoarvo rekisterieditorissa 1-asetukseksi HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.In the registry editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Kirjaudu RDS-palvelimessa ***sisään loppukäyttäjänä*** ja [varmista, että jaetun tietokoneen aktivointi on otettu käyttöön Microsoft 365 Apps for enterprise -sovelluksessa.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)

