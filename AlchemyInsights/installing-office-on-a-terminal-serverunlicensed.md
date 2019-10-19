---
title: Officen asentaminen Terminal Serveriin-käyttö oikeus ei ole lisensoitu
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
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/18/2019
ms.locfileid: "37205406"
---
# <a name="installing-office-on-a-terminal-server"></a>Officen asentaminen pääte palvelimeen

Jos haluat ottaa Office 365 ProPlusin käyttöön Windows Serverissä käyttämällä Remote Desktop Servicesiä (RDS), aiemmin nimettyjä pääte palveluita:
  
- Sinulla on oltava Office 365-suunnitelma, joka sisältää Office 365 ProPlusin, kuten Office 365 Enterprise E3 tai Enterprise E5. Office 365 Business-ja Office 365 Business Premium-paketit eivät sisällä Office 365 ProPlusia.

- Sinun on otettava käyttöön [jaetun tieto koneen Akti vointi](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Jos haluat asentaa Office 365 ProPlus RDS Microsoft 365 hallinta keskukseen, ***joka käyttää asennuksen oletus asetukset***, toimi seuraavasti.

> [!TIP]
> Voit myös ladata ja suorittaa [Microsoftin tuki-ja palautus avustajan](https://aka.ms/SaRA_OfficeSCA_M365Portal) ja asentaa Office 365 ProPlusin jaettuun tieto koneen aktivointi tilaan.
  
1. Tarkista, mitä Office 365-suunnitelma sinulla on. [Lue, miten](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Vaihda tarvittaessa toiseen Office 365-suunnitelmaan. [Lue, miten](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Jos Office on jo asennettu RDS-palvelimeen muiden Office 365-palvelu pakettien avulla, poista se. Esimerkiksi siirtymällä ohjaus paneeliin \> Poista ohjelma. Poista asennus [Microsoft Support-ja Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) -ohjelman avulla, jos ongelmia ei ole.

4. Kirjaudu RDS-palvelimella Microsoft 365-hallinta keskukseen järjestelmänvalvojan tilillä ja [Asenna Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).

5. Kun Office on asennettu, ***Älä avaa tai Kirjaudu*** mihinkään Office-sovelluksiin.

6. Ota käyttöön jaetun tieto koneen Akti vointi RDS-palvelimessa muokkaamalla rekisteriä tekemällä seuraavat toimet:

1. Napsauta hiiren kakkos painikkeella näytön vasemmassa alakulmassa olevaa Windows-painiketta ja valitse Suorita. Kirjoita Avaa-ruutuun **regedit**ja valitse sitten OK.

2. Valitse Kyllä, kun sinua pyydetään sallimaan rekisteri editorin tehdä muutoksia laitteeseesi.

3. Lisää rekisteri editorissa **Sharedcomputerlicensing** -merkki jono arvo, jonka asetus on 1 kohdassa HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Kirjaudu sisään RDS-palvelimessa ***loppu käyttäjänä*** ja [Varmista, että Office 365 ProPlusin jaetun tieto koneen Akti vointi on käytössä](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Lisä tietoja edellytyksistä, asennus ohjeista ja ohjeista mukautetuista asennuksista Officen käyttöönotto työkalun avulla on artikkelissa [office 365 ProPlusin käyttöönotto Etätyöpöytäpalvelujen avulla](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Voit korjata jaettuun tieto koneen Akti vointiin liittyviä virheitä kohdasta [Office 365 ProPlusin jaetun tieto koneen Akti voinnin ongelmien vian määritys](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  