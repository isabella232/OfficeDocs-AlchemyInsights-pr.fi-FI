---
title: Teams käyttöönotto erillisenä tai uusien tai olemassa olevien Office asennuksissa
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 6425b1eac3d5c99a6dfd227a1b445412c51a39b8
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320119"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Teams käyttöönotto erillisenä tai uusien tai olemassa olevien Office asennuksissa

Microsoft Teams sisältyy nyt uusien Microsoft 365 -sovellukset suuryrityksille,  Microsoft 365 -sovellukset yrityksille ja Office for Mac. Lisätietoja on kohdassa Milloin Microsoft Teams [tulee Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Ajantasaisen kanavan versiosta 1906 alkaen Teams lisätään  Microsoft 365 -sovellukset suuryrityksille (ja Microsoft 365 -sovellukset yrityksille) -asennuksiin laitteissa, joissa Windows on käytössä, kun päivität olemassa olevan asennuksen uusimpaan versioon. Lisätietoja on kohdassa Entä [nykyiset Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**Huomautus:** Jos et halua odottaa tätä käyttöönottoaikataulua, voit ottaa Teams käyttöön erillisenä käyttäjänä noudattamalla näitä ohjeita tai voit antaa käyttäjien asentaa Teams itse [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Jos organisaatiosi ei ole vielä Teams käyttöönottoon, voit poistaa Teams uusien ***tai*** olemassa [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) olevien [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) Office. Jos Teams asennettavaksi, mutta et halua, että Teams käynnistyy automaattisesti, kun se on asennettu, katso Microsoft Teams käynnistymisen estäminen asennuksen [jälkeen.](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)

Jos ***haluat Teams*** asennuksen laitteesta, jossa on Windows, katso lisätietoja [Microsoft Teams.](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81) Jos haluat Microsoft Teams useista kohdekoneista tai käyttäjistä, katso [lisätietoja Microsoft Teams käyttöönotosta.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

Jos käytät jaettuja tietokoneita, ETÄTYÖPÖYTÄpalveluja (RDS) tai Virtual Desktop Infrastructureia (VDI), katso jaetut tietokone- ja VDI-ympäristöt, joissa [on Microsoft Teams.](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)

Jos käytät Mac-Office for Mac, katso [Microsoft Teams asennuksia Macissa.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)

**Huomautus:** kun Teams on asennettu, se [](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) päivitetään automaattisesti noin kahden viikon välein uusilla ominaisuuksilla ja laatupäivityksillä. 