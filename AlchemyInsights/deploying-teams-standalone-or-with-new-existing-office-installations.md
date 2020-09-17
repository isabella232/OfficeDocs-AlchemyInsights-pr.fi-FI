---
title: Teamsin käyttöönotto erillisinä tai uusien tai olemassa olevien Office-asennusten avulla
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
ms.openlocfilehash: c3ca4365abc41509ccf602c5b9046655706840fc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806756"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Teamsin käyttöönotto erillisinä tai uusien tai olemassa olevien Office-asennusten avulla

Microsoft teams on nyt sisällytetty Microsoft 365-sovellusten, Microsoft 365-sovellusten yritys käyttöön ja Office for Macin ***uusiin asennuksiin*** . Lisä tietoja on kohdassa [Milloin Microsoft teams sisällytetään uusiin Office-asennuksiin?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Sen lisäksi, että versio 1906 on käytössä nykyisessä kanavassa, tiimit lisätään nykyisiin Microsoft 365 Apps for Enterprise (ja Microsoft 365-sovellukset yrityksille)- ***asennuksiin*** laitteissa, joissa on käytössä Windows, kun päivität nykyisen asennuksen uusimpaan versioon. Lisä tietoja on Ohje aiheessa [mitä on olemassa olevissa Office-asennuksissa?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Jos et halua odottaa tätä käyttöönotto aikataulua, voit ottaa käyttöön teamsin käyttäjiksi noudattamalla [näitä ohjeita](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)   tai voit määrittää käyttäjät asentamaan tiimit itse  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Jos organisaatiosi ei ole valmis ottamaan joukkueita käyttöön, voit ***poistaa teamsin*** [uusista](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) tai [nykyisistä](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) Office-asennuksista. Jos haluat, että tiimit asennetaan, mutta et halua, että tiimit käynnistyvät automaattisesti käyttäjän asennuksen jälkeen, Katso lisä tietoja artikkelista [Microsoft teamsin automaattisen käynnistymisen estäminen asentamisen jälkeen](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Lisä tietoja ***tiimien poistamisesta*** Windows-laitteesta on Ohje aiheessa [Microsoft teamsin asennuksen poistaminen](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Jos haluat puhdistaa Microsoft teamsin useista kohde koneista tai käyttäjistä, tutustu Ohje aiheeseen [Microsoft teamsin käyttöönoton puhdistaminen](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Jos käytät yhteiskäytössä olevia tieto koneita, Etätyöpöytäpalveluja (RDS) tai Virtual Desktop Infrastructure (VDI), tutustu Ohje aiheeseen jaettujen tieto koneiden ja VDI- [ympäristöjen käyttö Microsoft teamsissa](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Jos käytössäsi on Office for Mac, tutustu [Microsoft teamsin asennuksiin Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)-tieto koneessa.

> [!NOTE]
> Kun teamsin asennus on asennettu, se [päivittyy automaattisesti](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) noin kahden viikon välein uusilla ominaisuuksilla ja laatu päivityksillä. 