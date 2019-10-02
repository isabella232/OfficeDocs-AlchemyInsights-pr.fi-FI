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
ms.openlocfilehash: 6fc5645028c9fb9df2606c0d03b67e87ae15087c
ms.sourcegitcommit: 1e5de64e34e9ba16185b3a895b3152ca61718f4b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/01/2019
ms.locfileid: "37344235"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="f9a01-102">Ryhmien poistaminen uusista tai aiemmin luodusta Office-asennuksista tai niiden sulkeminen pois</span><span class="sxs-lookup"><span data-stu-id="f9a01-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="f9a01-103">Microsoft teams on nyt mukana osana Office 365 ProPlusia, Office 365 Business-ja Office for Mac-järjestelmiä.</span><span class="sxs-lookup"><span data-stu-id="f9a01-103">Microsoft Teams is now included as part of Office 365 ProPlus, Office 365 Business, and Office for Mac.</span></span>

- <span data-ttu-id="f9a01-104">Voit sulkea työryhmät pois uusista Office-asennuksista [Officen käyttöönotto työkalulla](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) .</span><span class="sxs-lookup"><span data-stu-id="f9a01-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="f9a01-105">Jos haluat poistaa teamsin *asennuksen* Windows-laitteesta, katso [Microsoft teamsin asennuksen poistaminen](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span><span class="sxs-lookup"><span data-stu-id="f9a01-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="f9a01-106">Jos haluat siivota Microsoft teamsin useista kohde koneista tai käyttäjistä, katso [Microsoft teams-käyttöönoton puhdistaminen](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span><span class="sxs-lookup"><span data-stu-id="f9a01-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="f9a01-107">Käytä [Preventteamsinstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) -vaihto ehtoa, jos haluat estää Microsoft teamsin asentavan automaattisesti Officen kanssa.</span><span class="sxs-lookup"><span data-stu-id="f9a01-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="f9a01-108">Käytä [Preventfirstlaunchafterinstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) -asetusta, *ennen kuin tiimit asennetaan*, jotta Microsoft teams ei käynnistynyt automaattisesti asennuksen jälkeen.</span><span class="sxs-lookup"><span data-stu-id="f9a01-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="f9a01-109">Jos käytössäsi on Office for Mac, katso [Microsoft teams-asennukset Macissa](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span><span class="sxs-lookup"><span data-stu-id="f9a01-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>