---
title: Poista Teamsin asennus tai jätä se pois Office-asennuksista
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
ms.openlocfilehash: 2d96d54cb479f5f52cc707d4307cf9cf1e891a01
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827789"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="4bcf2-102">Poista Teamsin asennus tai jätä se pois uusista tai olemassa olevista Office-asennuksista</span><span class="sxs-lookup"><span data-stu-id="4bcf2-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="4bcf2-103">Microsoft Teams sisältyy osana Microsoft 365 -sovelluksia yrityksille, Microsoft 365 -yrityssovelluksia ja Office for Macia.</span><span class="sxs-lookup"><span data-stu-id="4bcf2-103">Microsoft Teams is included as part of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span>

- <span data-ttu-id="4bcf2-104">Officen [käyttöönottotyökalun avulla voit](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) jättää Teamsin pois Officen uusista asennuksista.</span><span class="sxs-lookup"><span data-stu-id="4bcf2-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="4bcf2-105">Jos *haluat poistaa* Teamsin Windows-laitteesta, katso Microsoft [Teamsin asennuksen poistaminen.](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)</span><span class="sxs-lookup"><span data-stu-id="4bcf2-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="4bcf2-106">Jos haluat puhdistaa Microsoft Teamsin useista kohdekoneista tai käyttäjistä, katso [Microsoft Teamsin käyttöönoton puhdistus.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)</span><span class="sxs-lookup"><span data-stu-id="4bcf2-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="4bcf2-107">[PreventTeamsInstall-vaihtoehdon](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) avulla voit estää Microsoft Teamsia asentamasta officen kanssa automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="4bcf2-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="4bcf2-108">Käytä [PreventFirstLaunchAfterInstall-asetusta](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) ennen *Teamsin* asentamista, jotta Microsoft Teams ei käynnisty automaattisesti asennuksen jälkeen.</span><span class="sxs-lookup"><span data-stu-id="4bcf2-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="4bcf2-109">Jos käytät Office for Macia, katso [Lisätietoja on kohdassa Microsoft Teams -asennukset Mac-tietokoneessa.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)</span><span class="sxs-lookup"><span data-stu-id="4bcf2-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>