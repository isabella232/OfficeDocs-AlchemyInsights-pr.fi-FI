---
title: Office asennetaan päätepalvelin - varastettu
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 73d5128b55cae7712c48be9e2d05e558c3ba2e5c
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/24/2019
ms.locfileid: "29467717"
---
# <a name="installing-office-on-a-terminal-server"></a>Päätepalvelimen asennuksen

Voidaan ottaa käyttöön Office 365 ProPlus Windows-palvelimen käyttämällä Remote Desktop Services (RDS), nimeltään Terminal Services:
  
- Jos sinulla on Office 365-suunnitelma, joka sisältää Office 365 ProPlus, kuten Office 365 Enterprise-E3 tai yrityksen E5. Business Office 365: n ja Office 365: n Business Premium suunnitelmat eivät sisällä Office 365 ProPlus.
    
- On otettava käyttöön [jaettu tietokone aktivoiminen](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).
    
Jos haluat asentaa Office 365 ProPlus RDS Office 365-portaalista ** *asennuksesta oletusasetuksia käyttäen* **, toimi seuraavasti: 
  
1. Tarkista, mitä sinulla on Office 365-suunnitelma. [Tietoja siitä, miten](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. Jos tarpeen, siirry eri Office 365: ssä. [Tietoja siitä, miten](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. Jos RDS-palvelimeen, joka käyttää Office 365-suunnitelmat on jo asennettu Office, poista sen asennus. Esimerkiksi siirtymällä Ohjauspaneelin \> Poista ohjelman asennus. Asennuksen poisto käyttämällä [Microsoftin tuotetukeen ja palautus avustaja](https://aka.ms/SARA-OfficeUninstall-Alchemy) , jos ongelmia käytössä. 
    
4. RDS-palvelimen kirjautuminen järjestelmänvalvojana ja [Asenna Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx)Office 365-portaaliin.
    
5. Kun Office asennetaan, ** *ei avata tai kirjautua sisään* ** minkä tahansa Office-sovelluksiin. 
    
6. RDS-palvelimen käyttöön jaetun tietokoneen aktivointi muokkaamalla rekisteriä seuraavasti:
    
1. Napsauta näytön vasemmassa alakulmassa olevaa Windows-painiketta ja valitse Suorita. Kirjoita Avaa-ruutuun **regedit**ja valitse OK. 
    
2. Valitse Kyllä, kun kehotetaan sallimaan Registry Editor tehdä muutoksia laitteen.
    
3. Registry Editor Lisää merkkijonoarvo on **SharedComputerLicensing** , joka on asetettu 1 kohdassa HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration. 
    
7. RDS-palvelimeen ** *käyttäjä kirjautua* ** ja [Varmista, että jaetun tietokoneen aktivointi on käytössä Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).
    
Lisätietoja edellytykset, asennusohjeita ja ohjeita mukautettujen asennusten avulla Office Deployment Tool-työkalua on [Ottaa käyttöön Office 365 ProPlus Etätyöpöytäpalveluiden avulla](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Jaetun tietokoneen aktivointi liittyvien virheiden korjaamiseen on [jaetun tietokoneen aktivointi Office 365 ProPlus ongelmien vianmääritys](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  

