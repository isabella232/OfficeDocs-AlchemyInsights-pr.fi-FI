---
title: Officen asentaminen Terminal Serveriin-käyttöoikeudeton
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
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663114"
---
# <a name="installing-office-on-a-terminal-server"></a>Officen asentaminen pääte palvelimeen

Jos haluat ottaa käyttöön Microsoft 365-sovelluksia yritys käyttöön Windows-palvelimessa käyttämällä Etätyöpöytäpalveluja (RDS), aiemmin nimettyjä pääte palveluja:
  
- Sinulla on oltava Microsoft 365-tilaus, joka sisältää Microsoft 365-sovellukset yritykselle, kuten Office 365 Enterprise E3 tai Enterprise E5. Yritys käyttöön tarkoitettuja Microsoft 365-sovelluksia ja Microsoft 365-sovellukset eivät sisällä Microsoft 365-sovelluksia yritys käyttöön.

- Sinun on otettava käyttöön [jaettujen tieto koneiden Akti vointi](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Jos haluat asentaa Microsoft 365-sovelluksia Enterprise on RDS-sovellukseen Microsoft 365-hallinta keskuksesta, ***jossa käytetään oletusarvoisia asennus asetuksia***, noudata seuraavia ohjeita.

> [!TIP]
> Voit myös ladata ja suorittaa [Microsoftin tuki-ja palautus avustajan](https://aka.ms/SaRA_OfficeSCA_M365Portal) ja asentaa Microsoft 365-sovelluksia yritys käyttöön jaetussa tieto koneen aktivointi tilassa.
  
1. Tarkista, mikä Microsoft 365-tilaus sinulla on. [Lisä tietoja](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Vaihda tarvittaessa toiseen Microsoft 365-tila ukseen. [Lisä tietoja](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Jos Office on jo asennettu RDS-palvelimeen käyttämällä muita Microsoft 365-paketteja, poista sen asennus. Esimerkiksi siirtymällä ohjaus paneeliin voit \> poistaa ohjelman asennuksen. Poista asennus [Microsoftin tuki-ja palautus avustajan avulla,](https://aka.ms/SARA-OfficeUninstall-Alchemy) jos käytät ongelmia.

4. Kirjaudu RDS-palvelimessa Microsoft 365-hallinta keskukseen järjestelmänvalvojan tilillä ja [Asenna microsoft 365-sovellukset](https://portal.office.com/OLS/MySoftware.aspx)yrityksille.

5. Kun Office on asennettu, ***Älä avaa tai Kirjaudu sisään*** mihinkään Office-sovelluksiin.

6. Ota RDS-palvelimessa käyttöön tieto koneen yhteinen Akti vointi muokkaamalla rekisteriä noudattamalla seuraavia ohjeita:

1. Napsauta näytön vasemmassa alakulmassa olevaa Windows-painiketta hiiren kakkos painikkeella ja valitse Suorita. Kirjoita Avaa-ruutuun **regedit**ja valitse sitten OK.

2. Valitse Kyllä, kun ohjelma kysyy, sallitaanko rekisteri editorin tehdä muutoksia laitteeseesi.

3. Lisää rekisteri editorissa **Sharedcomputerlicensing** -arvo, jonka asetus on 1, HKEY_LOCAL_MACHINE \Microsoft\microsoft \Office\ClickToRun\Configuration.

7. Kirjaudu sisään RDS-palvelimessa ***loppu käyttäjänä*** ja [Varmista, että Microsoft 365-sovellukset on otettu käyttöön jaetussa tieto koneessa](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Lisä tietoja Office-käyttöönotto työkalun käyttö edellytyksistä, määritys ohjeista ja mukautetuista asennuksista on artikkelissa [Microsoft 365-sovellusten käyttöönotto yritys käyttöön tarkoitettuja Etätyöpöytäpalveluja](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)käyttämällä.
  
Jos haluat korjata jaettuihin tieto koneen Akti vointiin liittyviä ongelmia, Katso lisä tietoja artikkelista ongelmien [vian määritys jaetussa tieto koneessa Microsoft 365-sovellusten Akti vointi yrityksessä](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  