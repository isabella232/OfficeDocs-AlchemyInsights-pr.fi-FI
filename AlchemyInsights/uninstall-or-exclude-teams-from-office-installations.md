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
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="5226e-102">Uusien tai olemassa olevien Office-asennusten ryhmien poistaminen tai poissulkeminen</span><span class="sxs-lookup"><span data-stu-id="5226e-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="5226e-103">Microsoft teams kuuluu Microsoft 365-sovellusten yritys käyttöön, Microsoft 365 Apps for Businessiin ja Office for Maciin.</span><span class="sxs-lookup"><span data-stu-id="5226e-103">Microsoft Teams is included as part of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span>

- <span data-ttu-id="5226e-104">Käytä [Officen käyttöönotto työkalua](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) , jos haluat poistaa teamsin uusista Office-asennuksista.</span><span class="sxs-lookup"><span data-stu-id="5226e-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="5226e-105">Lisä tietoja tiimien *poistamisesta* Windows-laitteesta on Ohje aiheessa [Microsoft teamsin asennuksen poistaminen](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span><span class="sxs-lookup"><span data-stu-id="5226e-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="5226e-106">Jos haluat siivota Microsoft teams useista kohde koneista tai käyttäjistä, katso [Microsoft teamsin käyttöönoton puhdistaminen](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span><span class="sxs-lookup"><span data-stu-id="5226e-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="5226e-107">Käytä [Preventteamsinstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) -asetusta, jos haluat estää Microsoft teamsin asentamisen automaattisesti Officeen.</span><span class="sxs-lookup"><span data-stu-id="5226e-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="5226e-108">Estä Microsoft teamsin käynnistyminen automaattisesti asennuksen jälkeen, *ennen kuin tiimit on asennettu*, käyttämällä [Preventfireslaunchafterinstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) -asetusta.</span><span class="sxs-lookup"><span data-stu-id="5226e-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="5226e-109">Jos käytössäsi on Office for Mac, tutustu [Microsoft teamsin asennuksiin Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)-tieto koneessa.</span><span class="sxs-lookup"><span data-stu-id="5226e-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>