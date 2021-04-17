---
title: Microsoft 365 -sovelluksiin kirjautumisongelmat
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
- "9000571"
- "2574"
ms.openlocfilehash: 02841a1b4e92eec94fc6409941d91618f02518c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836600"
---
# <a name="issues-signing-into-microsoft-365-apps"></a><span data-ttu-id="f2bb7-102">Microsoft 365 -sovelluksiin kirjautumisongelmat</span><span class="sxs-lookup"><span data-stu-id="f2bb7-102">Issues signing into Microsoft 365 Apps</span></span>

<span data-ttu-id="f2bb7-103">Voit korjata Microsoft 365 -sovellusten kirjautumisongelmat kokeilemalla seuraavia vaihtoehtoja ongelmasta kärsivässä koneessa:</span><span class="sxs-lookup"><span data-stu-id="f2bb7-103">To fix sign-in issues with Microsoft 365 apps, try the following options on the affected machine:</span></span>  

- <span data-ttu-id="f2bb7-104">Windowsia koskevat [suositukset: Yleisimmät kirjautumisongelmat](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)</span><span class="sxs-lookup"><span data-stu-id="f2bb7-104">For Windows, see [Recommendations on resolving common sign-in issues](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)</span></span>
- <span data-ttu-id="f2bb7-105">Mac-tietokoneissa katso Office [2016 for Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail) -sovellukseen kirjautuminen ei toimi</span><span class="sxs-lookup"><span data-stu-id="f2bb7-105">For Mac, see  [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)</span></span>

<span data-ttu-id="f2bb7-106">**Vihje** Voimme diagnosoida ja korjata useita Windows-tietokoneiden Officen yleisiä sisäänkirjautumisongelmia puolestasi automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="f2bb7-106">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="f2bb7-107">Jos haluat käyttää automaattista työkaluamme, lataa ja suorita **[Microsoftin tuki- ja palautusavustaja](https://aka.ms/SaRA-OfficeSignInScenario)**.</span><span class="sxs-lookup"><span data-stu-id="f2bb7-107">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="f2bb7-108">**Huomautus:** Modernin varmennuksen (ADAL) tai WWW-tilin hallinnan (KÄYTTÖOIKEUKSIEN) käytöstä poistaminen kirjautumis- tai **aktivointiongelmiin ei ole suositeltavaa.**</span><span class="sxs-lookup"><span data-stu-id="f2bb7-108">**Note:** Disabling Modern Authentication (ADAL) or Web Account Management (WAM) for fixing sign-in or activation issues  **is not recommended**.</span></span> <span data-ttu-id="f2bb7-109">Jos virheitä ilmenee yhdistettäessä Microsoft 365:een Office 2013:n avulla, varmista, että otat modernin [todennuksen](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)  käyttöön Office-asiakasohjelmassa.</span><span class="sxs-lookup"><span data-stu-id="f2bb7-109">If the errors occur while connecting to Microsoft 365 using Office 2013, ensure that you [enable modern authentication](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)  for Office client.</span></span>

<span data-ttu-id="f2bb7-110">Lisätietoja vianmäärityksestä on kohdassa:</span><span class="sxs-lookup"><span data-stu-id="f2bb7-110">For specific troubleshooting actions, see:</span></span>

[<span data-ttu-id="f2bb7-111">Yhteysongelmat kirjautumisen yhteydessä Office 2016:n koontiversioon 16.0.7967 Windows 10:ssä</span><span class="sxs-lookup"><span data-stu-id="f2bb7-111">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[<span data-ttu-id="f2bb7-112">Et voi kirjautua organisaatiotiliisi, kuten Office 365:tä, Azurea tai Intunea.</span><span class="sxs-lookup"><span data-stu-id="f2bb7-112">You can't sign in to your organizational account such as Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[<span data-ttu-id="f2bb7-113">Muiden kuin selainsovellusten vianmääritys, jotka eivät voi kirjautua Office 365:ssä, Azuressa tai Intunessa</span><span class="sxs-lookup"><span data-stu-id="f2bb7-113">How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune</span></span>](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[<span data-ttu-id="f2bb7-114">Tunnistetietoja pyydetään toistuvasti Officessa</span><span class="sxs-lookup"><span data-stu-id="f2bb7-114">Repeatedly prompted for credentials in Office</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)