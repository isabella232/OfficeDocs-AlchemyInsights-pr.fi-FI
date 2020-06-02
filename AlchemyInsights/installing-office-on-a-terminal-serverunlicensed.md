---
title: Toimiston asentaminen päätepalvelimeen - Käyttöoikeudeton
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
ms.openlocfilehash: c781e9fd492ff97bc80667956e6609b3d40b28b4
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508625"
---
# <a name="installing-office-on-a-terminal-server"></a>Officen asentaminen päätepalvelimeen

Microsoft 365 -yrityssovellusten käyttöönotto Windows Serverissä etätyöpöytäpalveluiden (RDS) avulla, jotka olivat aiemmin nimeltään Päätepalvelut:
  
- Sinulla on oltava Microsoft 365 -tilaus, joka sisältää Microsoft 365 Apps for enterprise -sovelluksen, kuten Office 365 Enterprise E3:n tai Enterprise E5:n. Microsoft 365 -sovellukset yrityksille ja Microsoft 365 Apps for Business Premium -palvelupaketit eivät sisällä Microsoft 365 Apps for enterprise -sovelluksia.

- Sinun on otettava [jaetun tietokoneen aktivointi](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)käyttöön .

Jos haluat asentaa Microsoft 365 Apps for enterprise -sovellukset RDS:ään Microsoft 365 -hallintakeskuksesta, ***joka käyttää oletusasennusasetuksia,*** toimi seuraavasti.

> [!TIP]
> Voit myös ladata ja suorittaa [Microsoftin tuki- ja palautusavustajan](https://aka.ms/SaRA_OfficeSCA_M365Portal) ja asentaa Microsoft 365 Apps for enterprise -sovelluksen jaetun tietokoneen aktivointitilassa.
  
1. Tarkista, mikä Microsoft 365 -tilaus sinulla on. [Lue lisää](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Vaihda tarvittaessa toiseen Microsoft 365 -tilaukseen. [Lue lisää](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Jos Office on jo asennettu RDS-palvelimeen millä tahansa muulla Microsoft 365 -tilauksella, poista sen asennus. Jos esimerkiksi siirryt Ohjauspaneelin \> asennuksen poistamiseen. Poista asennus [Microsoftin tuki- ja palautusavustajan](https://aka.ms/SARA-OfficeUninstall-Alchemy) avulla, jos sinulla on ongelmia.

4. Kirjaudu RDS-palvelimessa Microsoft 365 -hallintakeskukseen järjestelmänvalvojan tilillä ja [asenna Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).

5. Kun Office on asennettu, ***älä avaa tai kirjaudu mihinkään*** Office-sovellukseen.

6. Ota jaetun tietokoneen aktivointi käyttöön RDS-palvelimessa muokkaamalla rekisteriä seuraavasti:

1. Napsauta näytön vasemmassa alakulmassa olevaa Windows-painiketta hiiren kakkospainikkeella ja valitse Suorita. Kirjoita Avaa-ruutuun **regedit**ja valitse sitten OK.

2. Valitse Kyllä, kun sinua kehotetaan antamaan Rekisterieditorin tehdä muutoksia laitteeseesi.

3. Lisää SharedComputerLicensing-merkkijonoarvo rekisterieditorissa 1-asetukseksi HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.In the registry editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Kirjaudu RDS-palvelimessa ***sisään loppukäyttäjänä*** ja [varmista, että jaetun tietokoneen aktivointi on otettu käyttöön Microsoft 365 Apps for enterprise -sovelluksessa.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)

Lisätietoja mukautettujen asennusten edellytyksistä, asennusohjeista ja ohjeista On [ohjeaiheessa Microsoft 365 -sovellusten käyttöönotto yrityksille etätyöpöytäpalveluiden avulla](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Lisätietoja jaetun tietokoneen aktivoinnin virheistä on [ohjeaiheessa Microsoft 365 Apps for enterprise -sovellusten jaetun tietokoneen aktivoinnin ongelmien vianmääritys](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  