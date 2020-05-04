---
title: Ryhmien asennuksen poistaminen office-asennuksista tai poistaminen siitä
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
ms.openlocfilehash: b6613733e743e08a9b18b1ada70fde164b0d5dc3
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010296"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="a5db4-102">Poista Teamsin asennus tai sulje se pois uusista tai aiemmin luoduista Office-asennuksista</span><span class="sxs-lookup"><span data-stu-id="a5db4-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="a5db4-103">Microsoft Teams sisältyy Microsoft 365 Apps for Enterprise -sovellukseen, Microsoft 365 Apps for Businessiin ja Office for Maciin.</span><span class="sxs-lookup"><span data-stu-id="a5db4-103">Microsoft Teams is included as part of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span>

- <span data-ttu-id="a5db4-104">[Officen käyttöönottotyökalun](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) avulla voit jättää Teamsin pois uusista Office-asennuksista.</span><span class="sxs-lookup"><span data-stu-id="a5db4-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="a5db4-105">Jos haluat poistaa Teamsin *asennuksen* Windows-laitteesta, katso [Microsoft Teamsin asennuksen poistaminen](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span><span class="sxs-lookup"><span data-stu-id="a5db4-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="a5db4-106">Lisätietoja Microsoft Teamsin puhdistaminen useista kohdekoneista tai käyttäjistä on ohjeaiheessa [Microsoft Teamsin käyttöönoton puhdistaminen](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span><span class="sxs-lookup"><span data-stu-id="a5db4-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="a5db4-107">Estä [TeamsInstall-vaihtoehdon](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) avulla voit estää Microsoft Teamsia asentamasta officea automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="a5db4-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="a5db4-108">Estä Microsoft Teamsin automaattinen käynnistyminen asennuksen jälkeen [PreventFirstLaunchAfterInstall-vaihtoehdon](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) *avulla, ennen kuin Teams asennetaan.*</span><span class="sxs-lookup"><span data-stu-id="a5db4-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="a5db4-109">Jos käytät Office for Macia, tutustu [ohjeaiheeseen Microsoft Teamsin asennukset Macissa](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span><span class="sxs-lookup"><span data-stu-id="a5db4-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>