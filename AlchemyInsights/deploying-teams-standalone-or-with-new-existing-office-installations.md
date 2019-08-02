---
title: Käyttöönotto ryhmien yksittäisenä tai uuteen tai aiemmin luotuun Office-asennukset
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 08/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 3318e1b17cc99e927e1011f7ca9eca8dec616d59
ms.sourcegitcommit: 4600dd4fb577bf5f5482a24616c2d9a6b81e8052
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/01/2019
ms.locfileid: "36054228"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Käyttöönotto ryhmien yksittäisenä tai uuteen tai aiemmin luotuun Office-asennukset

Microsoftin Teams on nyt sisällytetty osana ***uusien asennusten*** Office 365 ProPlus Business Office 365: n ja Office for Macissa. Lisätietoja on ohjeaiheessa [Kun Microsoftin Teams aloitetaan parhaillaan mukana uusien asennusten Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

Lisäksi kuukausittain kanavassa versio 1906 alkaen ryhmiä on Office 365 ProPlus (ja Office 365-Business) ***lisätään olemassa olevien laitosten*** laitteissa, joissa Windows, kun päivität aiemman asennuksen uusimpaan versioon. Lisätietoja on ohjeaiheessa [mitä tietoja Office aiemmat asennukset?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> Jos et halua odottaa tätä aikataulua rahoittaja, voit ottaa käyttöön ryhmien yksittäisenä käyttäjiä varten noudattamalla [seuraavia ohjeita](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) tai voit antaa käyttäjien ryhmät asentaminen itse [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).

Jos organisaatiosi ei ole valmis ottamaan ryhmiä, meillä on toimet voidaan jättää ***ryhmien*** laitosten [uuteen](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) tai [aiemmin luotuun](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) Office. Jos haluat ryhmien asennettu, mutta et haluat ryhmien käynnistymään automaattisesti käyttäjän, kun se on asennettu, katso [Microsoftin työryhmät estä käynnistymästä automaattisesti asennuksen jälkeen](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Lisätietoja Windows-laitteesta ***poistaa ryhmiä*** , [Poistaa Microsoftin työryhmät](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Uudelleenjärjestäminen Microsoft Teamsien useista kohdetietokoneessa tai käyttäjien on [Microsoftin työryhmät käyttöönoton tyhjennys](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Jos käytät jaettuja tietokoneita, Remote Desktop Services (RDS) tai Virtual Desktop Infrastructure (VDI), on [jaettu tietokone ja VDI-ympäristöissä, joissa Microsoftin työryhmät](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Jos käytät Office for Mac on [Mac Microsoftin työryhmät laitosta](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Kun ryhmät on asennettu, se on [päivitetään automaattisesti](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) noin kahden viikon välein uusia ominaisuuksia ja päivityksiä laatua. 