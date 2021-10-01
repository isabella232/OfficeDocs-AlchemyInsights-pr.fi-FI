---
title: Rds Microsoft 365 -sovellukset, päätepalvelimen tai VDI:n jaettua käyttöä varten käyttöönotettaessa
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
ms.openlocfilehash: 81183cf1823480c1b15eba9ba9f519b4e3746b52
ms.sourcegitcommit: ef8d6b71fbd962fb3f7081b21724e67a91111a92
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/01/2021
ms.locfileid: "60077247"
---
# <a name="deploying-microsoft-365-apps-for-shared-use-on-rds-terminal-server-or-vdi"></a>Rds Microsoft 365 -sovellukset, päätepalvelimen tai VDI:n jaettua käyttöä varten käyttöönotettaessa

Jos haluat Microsoft 365 -sovellukset etätyöpöytäpalveluja (RDS) käyttäen päätepalveluja, sinun on

- Ota TLS 1.2 käyttöön oletusarvoisesti helpon korjauksen avulla, jos käytössäsi on Windows-versio (esimerkiksi Windows 7 SP1 tai Windows Server 2008 R2). Lisätietoja on Windows 36:n WinHTTP in Windows -sovelluksen päivityksessä, jossa [TLS 1.1 ja TLS 1.2](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy)otetaan käyttöön oletusturvallisina protokollina. 
- Sinulla on suunnitelma, joka sisältää Microsoft 365 -sovellukset suuryrityksille (aiemmin Office 365 Plus). Esimerkiksi Office 365 E3 Microsoft 365 E5 tai mikä tahansa suunnitelma, joka sisältää Project tai Visio työpöytäversion, kuten Project (palvelupaketti 3) tai Visio (palvelupaketti 2), tai Microsoft 365 Business Premium, joka sisältää myös Microsoft 365 -sovellukset yrityksille.
- Ota käyttöön jaetun tietokoneen aktivointi. Lisätietoja on kohdassa Yleistä jaetun [tietokoneen aktivoinnista Microsoft 365 -sovellukset.](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation)

**Huomautus:** Jos haluat Microsoft 365 -sovellukset jaetun tietokoneen aktivointitilaan, lataa ja suorita [Microsoft tuki- ja palautusavustaja.](https://aka.ms/SaRA_OfficeSCA_M365Portal) Lisätietoja edellytyksistä, asennusohjeista ja asennusten mukauttamisesta Office-käyttöönottotyökalun avulla on kohdassa [Microsoft 365 -sovellukset käyttöönotto etätyöpöytäpalvelujen avulla.](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services)

Lisätietoja jaetun tietokoneen aktivointiin liittyvien virheiden korjaamisesta on kohdassa:

- [Jaetun tietokoneen aktivointiongelmien vianmääritys Microsoft 365 -sovellukset](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [Palauta aktivointitila Microsoft 365 -yrityssovelluksille.](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

Jos haluat asentaa Microsoft 365 -sovellukset RDS-Microsoft 365 -hallintakeskus, joka käyttää oletusasennusasetuksia, toimi seuraavasti:

1. Tarkista Microsoft 365 suunnitelmasi. Lisätietoja on kohdassa [Mikä tilaus minulla on?](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).

1. Vaihda tarvittaessa toiseen Microsoft 365. Lisätietoja on kohdassa [Toiseen suunnitelmaan päivittäminen.](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan)

1. Jos Microsoft 365 -sovellukset RDS-palvelimeen käyttämällä muita yhteensopimattomia palvelupaketteja, poista sen asennus valitsemalla **Ohjauspaneelin Poista**  >  **ohjelman asennus**. Jos ongelmia tulee, poista asennus lataamalla [Microsoft tuki- ja palautusavustaja.](https://aka.ms/SARA-OfficeUninstall-Alchemy)

1. Kirjaudu RDS-palvelimessa Microsoft 365 -hallintakeskus järjestelmänvalvojan tilillä ja asenna [Office.](https://portal.office.com/OLS/MySoftware.aspx)

   Kun Office on asennettu, älä avaa tai kirjaudu sisään Office sovelluksiin.

1. Ota RDS-palvelimessa käyttöön jaetun tietokoneen aktivointi muokkaamalla rekisteriä:

   1. Napsauta hiiren Windows näytön vasemmassa alakulmassa olevaa Windows-painiketta ja valitse **Suorita**. Kirjoita Avaa-ruutuun **regedit** ja napsauta sitten **OK**.

   1. Kun sinua pyydetään sallimaan Rekisterieditorin tehdä muutoksia laitteeseesi, valitse **Kyllä**.

   1. Lisää Rekisterieditorin HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration-kohdassa **Jaetun täydennyksen** käyttöoikeuden merkkijonoarvo, jonka asetus on **1.**

1. Kirjaudu RDS-palvelimessa sisään käyttäjänä ja varmista, että jaetun tietokoneen aktivointi on otettu käyttöön Microsoft 365 -sovellukset. 

   Lisätietoja on kohdassa [Jaetun tietokoneen aktivoinnin tarkistaminen Microsoft 365 -sovellukset.](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps)