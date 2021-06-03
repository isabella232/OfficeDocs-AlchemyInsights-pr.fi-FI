---
title: Päätepiste DLP:tä ei ole otettu käyttöön käyttäjän laitteessa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731411"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a><span data-ttu-id="1164a-102">Päätepiste DLP:tä ei ole otettu käyttöön käyttäjän laitteessa</span><span class="sxs-lookup"><span data-stu-id="1164a-102">Endpoint DLP not deployed to user's device</span></span>

<span data-ttu-id="1164a-103">Jos Endpoint-tietojen menetyksen estämisasetus (DLP) ei ole käytössä käyttäjän laitteessa, varmista, että täytät seuraavat vaatimukset:</span><span class="sxs-lookup"><span data-stu-id="1164a-103">If the Endpoint data loss prevention (DLP) setting has not applied to a user's device, confirm you meet these requirements:</span></span>

- <span data-ttu-id="1164a-104">Windows 10 x64 koontiversio 1809 tai uudempi on asennettu laitteeseen.</span><span class="sxs-lookup"><span data-stu-id="1164a-104">Windows 10 x64 build 1809 or later is installed on the device.</span></span>
- <span data-ttu-id="1164a-105">Haittaohjelmien torjuntaohjelman versio 4.18.2009.7 tai uudempi on asennettu.</span><span class="sxs-lookup"><span data-stu-id="1164a-105">Anti-malware client version 4.18.2009.7 or later is installed.</span></span>
- <span data-ttu-id="1164a-106">Laite on **jokin** seuraavista:</span><span class="sxs-lookup"><span data-stu-id="1164a-106">The device is **one** of these:</span></span>
    
    - <span data-ttu-id="1164a-107">Azure Active Directory (Azure AD) liitetty</span><span class="sxs-lookup"><span data-stu-id="1164a-107">Azure Active Directory (Azure AD) joined</span></span>
    - <span data-ttu-id="1164a-108">Azure AD -yhdistelmäympäristö liitetty</span><span class="sxs-lookup"><span data-stu-id="1164a-108">Hybrid Azure AD joined</span></span>
    - <span data-ttu-id="1164a-109">Rekisteröity AAD</span><span class="sxs-lookup"><span data-stu-id="1164a-109">AAD registered</span></span>

- <span data-ttu-id="1164a-110">Jos haluat pakottaa käytäntötoiminnot, varmista, että Microsoft Chromium Edge -selain on asennettu päätepistelaitteeseen.</span><span class="sxs-lookup"><span data-stu-id="1164a-110">To enforce policy actions, make sure Microsoft Chromium Edge browser is installed on the endpoint device.</span></span>

<span data-ttu-id="1164a-111">Lisätietoja Endpoint DLP:n käyttöönottovaatimuksista on kohdassa [Endpoint-tietojen menetyksen estämisen käytön aloittaminen.](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)</span><span class="sxs-lookup"><span data-stu-id="1164a-111">For additional requirements for deploying Endpoint DLP, see [Get started with Endpoint data loss prevention](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span></span>