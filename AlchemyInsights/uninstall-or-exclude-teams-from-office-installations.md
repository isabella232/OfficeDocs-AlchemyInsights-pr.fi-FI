---
title: Teamsin poistaminen tai poissulkeminen Office-asennuksista
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: 22d69db749671afdfe7a809d1bc598e2ad1891d8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658218"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>Uusien tai olemassa olevien Office-asennusten ryhmien poistaminen tai poissulkeminen

Microsoft teams kuuluu Microsoft 365-sovellusten yritys käyttöön, Microsoft 365 Apps for Businessiin ja Office for Maciin.

- Käytä [Officen käyttöönotto työkalua](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) , jos haluat poistaa teamsin uusista Office-asennuksista.
- Lisä tietoja tiimien *poistamisesta* Windows-laitteesta on Ohje aiheessa [Microsoft teamsin asennuksen poistaminen](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Jos haluat siivota Microsoft teams useista kohde koneista tai käyttäjistä, katso [Microsoft teamsin käyttöönoton puhdistaminen](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).
- Käytä [Preventteamsinstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) -asetusta, jos haluat estää Microsoft teamsin asentamisen automaattisesti Officeen.
- Estä Microsoft teamsin käynnistyminen automaattisesti asennuksen jälkeen, *ennen kuin tiimit on asennettu*, käyttämällä [Preventfireslaunchafterinstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) -asetusta.

Jos käytössäsi on Office for Mac, tutustu [Microsoft teamsin asennuksiin Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)-tieto koneessa.