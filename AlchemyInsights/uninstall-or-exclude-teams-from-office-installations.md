---
title: Ryhmien poistaminen tai poissulkeminen Office-asennuksista
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: c6d5c0233acb8fb71127dcb54c719b71aa1a5bcb
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/29/2019
ms.locfileid: "37769804"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>Ryhmien poistaminen uusista tai aiemmin luodusta Office-asennuksista tai niiden sulkeminen pois

Microsoft teams sisältyy Office 365 ProPlus-, Office 365 Business-ja Office for Mac-pakettiin.

- Voit sulkea työryhmät pois uusista Office-asennuksista [Officen käyttöönotto työkalulla](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) .
- Jos haluat poistaa teamsin *asennuksen* Windows-laitteesta, katso [Microsoft teamsin asennuksen poistaminen](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Jos haluat siivota Microsoft teamsin useista kohde koneista tai käyttäjistä, katso [Microsoft teams-käyttöönoton puhdistaminen](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).
- Käytä [Preventteamsinstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) -vaihto ehtoa, jos haluat estää Microsoft teamsin asentavan automaattisesti Officen kanssa.
- Käytä [Preventfirstlaunchafterinstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) -asetusta, *ennen kuin tiimit asennetaan*, jotta Microsoft teams ei käynnistynyt automaattisesti asennuksen jälkeen.

Jos käytössäsi on Office for Mac, katso [Microsoft teams-asennukset Macissa](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).