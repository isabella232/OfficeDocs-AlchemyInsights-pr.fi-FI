---
title: Asennuksen poistaminen tai Teams poistaminen Office asennuksista
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: a960c96abf6215e3a34908ce8669a0c61298daac829343b3673dbfef0c4cbfc7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007715"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>Poista tai jätä Teams uusista tai olemassa olevista Office asennuksista

Microsoft Teams sisältyy Microsoft 365 -sovellukset suuryrityksille, Microsoft 365 -sovellukset yrityksille ja Office for Mac.

- Voit [Office käyttöönottotyökalun avulla,](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) Teams ei sisälly Office.
- Jos *haluat* Teams asennuksen laitteesta, jossa on Windows, katso [lisätietoja Microsoft Teams.](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81) Jos haluat Microsoft Teams useista kohdekoneista tai käyttäjistä, katso [Microsoft Teams puhdistaminen.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)
- [PreventTeamsInstall-vaihtoehdon](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) avulla voit estää Microsoft Teams automaattisen asennuksen Office.
- Käytä [PreventFirstLaunchAfterInstall-Teams](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) *ennen* Microsoft Teams -asetusta, jos haluat estää Microsoft Teams automaattisen käynnistymisen asennuksen jälkeen.

Jos käytät Windows-Office for Mac, katso [Microsoft Teams asennuksia Macissa.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)