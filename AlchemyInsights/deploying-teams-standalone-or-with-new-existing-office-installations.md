---
title: Ryhmien käyttöönotto erillisinä tai uusilla tai olemassa olevilla Office-asennuksilla
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
ms.openlocfilehash: 5ec5277a758fc5171c846266787c2fbcf751f21c
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/09/2020
ms.locfileid: "44617892"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Ryhmien käyttöönotto erillisinä tai uusilla tai olemassa olevilla Office-asennuksilla

Microsoft Teams sisältyy nyt microsoft 365 -yrityssovellusten, Microsoft 365 Apps for Businessin ja Office for Macin ***uusiin asennuksiin.*** Lisätietoja on [ohjeaiheessa Milloin Microsoft Teams alkaa sisältyä uusiin Office-asennuksiin?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Lisäksi Nykyisellä kanavalla versiosta 1906 alkaen Teams lisätään Microsoft 365 Apps for enterprise (ja Microsoft 365 Apps for Business) ***-asennuksiin*** Windows-laitteissa, kun päivität aiemmin luodun asennuksen uusimpaan versioon. Lisätietoja on ohjeaiheessa [Entä officen nykyiset asennukset?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Jos et halua odottaa tätä käyttöönottoaikataulua, voit ottaa Teamsin käyttöön erillisenä käyttäjänä [noudattamalla näitä ohjeita](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)   tai voit pyytää käyttäjiä asentamaan Teamsin itse  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) -asennuksesta.

Jos organisaatiosi ei ole valmis ottamaan Teamjä käyttöön, voit ***estää Teamsin pois*** [uusista](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) tai [olemassa olevista](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) Office-asennuksista. Jos haluat, että Teams asennetaan, mutta et halua, että Teams käynnistyy automaattisesti käyttäjälle asennuksen jälkeen, katso [Lisätietoja artikkelista Microsoft Teamsin automaattisen käynnistymisen estäminen asennuksen jälkeen](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Lisätietoja ***Teamsin poistamisesta*** Windows-laitteesta on ohjeaiheessa [Microsoft Teamsin asennuksen poistaminen](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Lisätietoja Microsoft Teamsin puhdistamiseksi useista kohdekoneista tai käyttäjistä on ohjeaiheessa [Microsoft Teamsin käyttöönoton siivoaminen](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Jos käytössäsi on jaettuja tietokoneita, RDS (Remote Desktop Services) -palveluita tai VDI (Virtual Desktop Infrastructure) -infrastruktuuria, katso [jaetut tietokone- ja VDI-ympäristöt Microsoft Teamsin kanssa](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Jos käytät Office for Macia, katso Microsoft [Teamsin asennukset Macissa](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Kun Teams on asennettu, se [päivittyy automaattisesti](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) noin kahden viikon välein uusilla ominaisuuksilla ja laatupäivityksillä. 