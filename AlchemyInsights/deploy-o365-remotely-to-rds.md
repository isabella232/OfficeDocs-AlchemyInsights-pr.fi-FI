---
title: Microsoft 365-sovellusten käyttöönotto yritys käyttöön jaetussa käytössä RDS-, Terminal Server-tai VDI-sovelluksissa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 22ded616e82b2e82023b55a1d3ca6251cfb71712
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745532"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Microsoft 365-sovellusten käyttöönotto yritys käyttöön jaetussa käytössä RDS-, Terminal Server-tai VDI-sovelluksissa

Jos haluat ottaa käyttöön Microsoft 365-sovelluksia yrityksille käyttämällä Etätyöpöytäpalveluja (RDS), aiemmin nimettyjä pääte palveluja:
- Sinulla on oltava Microsoft 365 for Business-tilaus tai Office 365-tilaus, joka sisältää Microsoft 365 Enterprise-sovellukset, kuten Office 365 Enterprise E3 tai Enterprise E5.
   > [!NOTE] 
   > Microsoft 365-sovellukset yrityksille-ja Microsoft 365 Business Premium Standard-palvelu paketit eivät sisällä Microsoft 365-sovelluksia yritys käyttöön.
- Sinun on otettava käyttöön [jaettujen tieto koneiden Akti vointi](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Voit myös ladata ja suorittaa [Microsoftin tuki-ja palautus avustajan](https://aka.ms/SaRA_OfficeSCA_M365Portal) ja asentaa Microsoft 365-sovelluksia yritys käyttöön jaetussa tieto koneen aktivointi tilassa.

Lisä tietoja Office-käyttöönotto työkalun käyttö edellytyksistä, määritys ohjeista ja mukautetuista asennuksista on artikkelissa [Microsoft 365-sovellusten käyttöönotto yritys käyttöön tarkoitettuja Etätyöpöytäpalveluja](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)käyttämällä.

Voit korjata jaettuihin tieto koneen Akti vointiin liittyvät virheet toimimalla seuraavasti:
- Katso lisä tietoja artikkelista ongelmien [vian määritys jaetussa tieto koneessa Microsoft 365-sovellusten Akti vointi](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)yrityksille.
- Katso [Palauta aktivointitila Microsoft 365 -yrityssovelluksille](https://go.microsoft.com/fwlink/?linkid=2109218).

Jos haluat asentaa Microsoft 365-sovelluksia Enterprise on RDS-sovellukseen Microsoft 365-hallinta keskuksesta, jossa on käytössä ***oletusarvoiset asennus asetukset***, noudata seuraavia ohjeita:

1.    Tarkista, mikä tilaus sinulla on. [Ohjeet](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2.    Vaihda tarvittaessa toiseen tila ukseen. [Ohjeet](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3.    Jos Office on jo asennettu RDS-palvelimeen muilla Microsoft-paketeillä, poista sen asennus. Esimerkiksi siirtymällä **ohjaus paneeliin**voit  >  **poistaa ohjelman asennuksen**. Poista asennus [Microsoftin tuki-ja palautus avustajan avulla,](https://aka.ms/SARA-OfficeUninstall-Alchemy) jos käytät ongelmia.
4.    Kirjaudu RDS-palvelimessa Microsoft 365-hallinta keskukseen järjestelmänvalvojan tilillä ja [Asenna microsoft 365-sovellukset](https://portal.office.com/OLS/MySoftware.aspx)yrityksille.
5.    Kun Office on asennettu, ***Älä avaa tai Kirjaudu sisään*** mihinkään Office-sovelluksiin.
6.    Ota RDS-palvelimessa käyttöön tieto koneen yhteinen Akti vointi muokkaamalla rekisteriä noudattamalla seuraavia ohjeita:
   1. Napsauta näytön vasemmassa alakulmassa olevaa Windows-painiketta hiiren kakkos painikkeella ja valitse **Suorita**. Kirjoita Avaa-ruutuun **regedit**ja valitse sitten **OK**.
   2. Valitse **Kyllä** , kun ohjelma kysyy, sallitaanko rekisteri editorin tehdä muutoksia laitteeseesi.
   3. Lisää rekisteri editorissa **Sharedcomputerlicensing** -arvo, jonka asetus on 1, HKEY_LOCAL_MACHINE \Microsoft\microsoft \Office\ClickToRun\Configuration.
   4. Kirjaudu sisään RDS-palvelimessa ***loppu käyttäjänä*** ja [Varmista, että Microsoft 365-sovellukset on otettu käyttöön jaetussa tieto koneessa](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

