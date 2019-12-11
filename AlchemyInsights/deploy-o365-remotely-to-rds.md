---
title: Office 365 ProPlusin käyttöönotto jaettuun käyttöön RDS-, Terminal Server-tai VDI-palvelimessa
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959457"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a>Office 365 ProPlusin käyttöönotto jaettuun käyttöön RDS-, Terminal Server-tai VDI-palvelimessa

Voit ottaa Office 365 ProPlusin käyttöön käyttämällä Remote Desktop Servicesia (RDS), jonka nimi oli aiemmin Terminal Services:
- Sinulla on oltava Microsoft 365 for Business-suunnitelma tai Office 365-suunnitelma, joka sisältää Office 365 ProPlusin, kuten Office 365 Enterprise E3 tai Enterprise E5.
   > [!NOTE] 
   > Office 365 Business-ja Office 365 Business Premium-paketit eivät sisällä Office 365 ProPlusia.
- Sinun on otettava käyttöön [jaetun tieto koneen Akti vointi](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> Voit myös ladata ja suorittaa [Microsoftin tuki-ja palautus avustajan](https://aka.ms/SaRA_OfficeSCA_M365Portal) ja asentaa Office 365 ProPlusin jaettuun tieto koneen aktivointi tilaan.

Lisä tietoja edellytyksistä, asennus ohjeista ja mukautettujen asennusten ohjeista Officen käyttöönotto työkalun avulla on artikkelissa [office 365 ProPlusin käyttöönotto Etätyöpöytäpalvelujen avulla](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

Jaettuun tieto koneen Akti vointiin liittyvien virheiden korjaaminen:
- Katso [Office 365 ProPlusin jaetun tieto koneen Akti voinnin ongelmien vian määritys](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Katso [Office 365 ProPlus-aktivointi tilan palauttaminen](https://go.microsoft.com/fwlink/?linkid=2109218).

Jos haluat asentaa Office 365 ProPlus RDS Microsoft 365 hallinta keskukseen, ***joka käyttää asennuksen oletus asetukset***, toimi seuraavasti:

1.  Tarkista, mitä Office 365-suunnitelma sinulla on. [Ohjeet](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.  Vaihda tarvittaessa toiseen Office 365-suunnitelmaan. [Ohjeet](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.  Jos Office on jo asennettu RDS-palvelimeen muiden Office 365-palvelu pakettien avulla, poista se. Esimerkiksi siirtymällä **ohjaus paneeliin** > **Poista ohjelma**. Poista asennus [Microsoft Support-ja Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) -ohjelman avulla, jos ongelmia ei ole.
4.  Kirjaudu RDS-palvelimella Microsoft 365-hallinta keskukseen järjestelmänvalvojan tilillä ja [Asenna Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
5.  Kun Office on asennettu, ***Älä avaa tai Kirjaudu*** mihinkään Office-sovelluksiin.
6.  Ota käyttöön jaetun tieto koneen Akti vointi RDS-palvelimessa muokkaamalla rekisteriä tekemällä seuraavat toimet:
   1. Napsauta hiiren kakkos painikkeella näytön vasemmassa alakulmassa olevaa Windows-painiketta ja valitse **Suorita**. Kirjoita Avaa-ruutuun **regedit**ja valitse sitten **OK**.
   2. Valitse **Kyllä** , kun sinua pyydetään sallimaan rekisteri editorin tehdä muutoksia laitteeseesi.
   3. Lisää rekisteri editorissa **Sharedcomputerlicensing** -merkki jono arvo, jonka asetus on 1 kohdassa HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Kirjaudu sisään RDS-palvelimessa ***loppu käyttäjänä*** ja [Varmista, että Office 365 ProPlusin jaetun tieto koneen Akti vointi on käytössä](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

