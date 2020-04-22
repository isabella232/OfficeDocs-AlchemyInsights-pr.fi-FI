---
title: Teamsin käyttöönotto itsenäisenä tai uusien tai aiemmin luotujen Office-asennusten avulla
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 4b843407f05db207f3b676c03c7088d3d0ba062e
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704630"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Teamsin käyttöönotto itsenäisenä tai uusien tai aiemmin luotujen Office-asennusten avulla

Microsoft Teams sisältyy nyt Microsoft 365 Apps for Enterprise-, Microsoft 365 Apps for Business- ja Office for Mac ***-versioihin.*** Lisätietoja on ohjeaiheessa [Milloin Microsoft Teams alkaa sisältyä uusiin Office-asennuksiin?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

Lisäksi, alkaen versiosta 1906 Monthly Channelissa, Teams lisätään olemassa oleviin Microsoft 365 Apps for enterprise (ja Microsoft 365 Apps for Business) ***-asennuksiin*** Windows-laitteissa, kun päivität nykyisen asennuksen uusimpaan versioon. Lisätietoja on [ohjeaiheessa Entä olemassa olevat Office-asennukset?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> Jos et halua odottaa tätä käyttöönottoaikataulua, voit ottaa Teamsin käyttöön erillisinä käyttäjillesi [noudattamalla näitä ohjeita](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads)tai voit antaa käyttäjien asentaa Teamsin itse -kohdasta .

Jos organisaatiosi ei ole valmis ottamaan Teamsia käyttöön, meillä on ohjeet, joilla voit ***sulkea Teamsin pois*** [uusista](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) tai [olemassa olevista](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) Office-asennuksista. Jos haluat, että Teams asennetaan, mutta et halua Teamsiin käynnistyvan automaattisesti käyttäjän asennuksen jälkeen, katso lisätietoja ohjeaiheesta [Microsoft Teamsin automaattisen käynnistymisen estäminen asennuksen jälkeen](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Jos haluat ***poistaa Teamsin asennuksen*** Windows-laitteesta, katso [Microsoft Teamsin asennuksen poistaminen](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Lisätietoja Microsoft Teamsin puhdistaminen useista kohdekoneista tai käyttäjistä on ohjeaiheessa [Microsoft Teamsin käyttöönoton puhdistaminen](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Jos käytät jaettuja tietokoneita, etätyöpöytäpalveluja (RDS) tai Näennäistyöpöytäinfrastruktuuria (VDI), katso [Jaetut tietokoneet ja VDI-ympäristöt Microsoft Teamsin kanssa](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Jos käytät Office for Macia, tutustu [ohjeaiheeseen Microsoft Teamsin asennukset Macissa](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Kun Teams on asennettu, se [päivittyy automaattisesti](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) noin kahden viikon välein uusilla ominaisuuksilla ja laatupäivityksillä. 