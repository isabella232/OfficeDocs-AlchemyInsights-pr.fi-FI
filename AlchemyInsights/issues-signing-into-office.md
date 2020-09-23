---
title: Ongelmia, jotka liittyvät Microsoft 365-sovelluksiin kirjautumiseen
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
- "9000571"
- "2574"
ms.openlocfilehash: a1e9844094dd164ca8bd5fb2a196161a5de0282f
ms.sourcegitcommit: 57102d7daf32f370cab84dba342819a1ad5cb261
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/23/2020
ms.locfileid: "48236122"
---
# <a name="issues-signing-into-microsoft-365-apps"></a><span data-ttu-id="29f33-102">Ongelmat kirjautumisessa Microsoft 365-sovelluksiin</span><span class="sxs-lookup"><span data-stu-id="29f33-102">Issues signing into Microsoft 365 Apps</span></span>

<span data-ttu-id="29f33-103">Jos haluat korjata kirjautumisongelmat Microsoft 365-sovelluksissa, kokeile seuraavia vaihto ehtoja haavoittuvuuden sisältävään tieto koneeseen:</span><span class="sxs-lookup"><span data-stu-id="29f33-103">To fix sign-in issues with Microsoft 365 apps, try the following options on the affected machine:</span></span>  

- <span data-ttu-id="29f33-104">Windowsissa on ohjeet [yleisten kirjautumisongelmien ratkaisemiseen](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues) .</span><span class="sxs-lookup"><span data-stu-id="29f33-104">For Windows, see [Recommendations on resolving common sign-in issues](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)</span></span>
- <span data-ttu-id="29f33-105">Katso lisä tietoja artikkelista  [Kirjautuminen Office 2016 for Mac-sovellukseen ei onnistu](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)</span><span class="sxs-lookup"><span data-stu-id="29f33-105">For Mac, see  [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)</span></span>

<span data-ttu-id="29f33-106">**Vinkki** Windows-koneilla voimme diagnosoida ja korjata automaattisesti useita tavallisia Officen kirjautumisongelmia.</span><span class="sxs-lookup"><span data-stu-id="29f33-106">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="29f33-107">Lataa ja suorita  **[Microsoftin tuki-ja palautus avustaja](https://aka.ms/SaRA-OfficeSignInScenario)** , jotta voit käyttää automaattista työkalua.</span><span class="sxs-lookup"><span data-stu-id="29f33-107">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="29f33-108">**Huomautus:** Modernin todentamisen (ADAL) tai verkko tilin hallinnan (WAM) poistamista käytöstä kirjautumis-tai aktivointi ongelmien korjaamiseksi ei  **suositella**.</span><span class="sxs-lookup"><span data-stu-id="29f33-108">**Note:** Disabling Modern Authentication (ADAL) or Web Account Management (WAM) for fixing sign-in or activation issues  **is not recommended**.</span></span> <span data-ttu-id="29f33-109">Jos virhe ilmenee, kun muodostat yhteyden Microsoft 365-palveluun Office 2013-sovelluksen avulla, varmista, että olet [ottanut käyttöön modernin todentamisen](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)  Office-asiakas ohjelmassa.</span><span class="sxs-lookup"><span data-stu-id="29f33-109">If the errors occur while connecting to Microsoft 365 using Office 2013, ensure that you [enable modern authentication](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)  for Office client.</span></span>

<span data-ttu-id="29f33-110">Lisä tietoja vian määritys toiminnoista on kohdassa:</span><span class="sxs-lookup"><span data-stu-id="29f33-110">For specific troubleshooting actions, see:</span></span>

[<span data-ttu-id="29f33-111">Yhteysongelmat kirjautumisen yhteydessä Office 2016:n koontiversioon 16.0.7967 Windows 10:ssä</span><span class="sxs-lookup"><span data-stu-id="29f33-111">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[<span data-ttu-id="29f33-112">Et voi kirja utua organisaatiosi tiliin, kuten Office 365, Azure tai Intune</span><span class="sxs-lookup"><span data-stu-id="29f33-112">You can't sign in to your organizational account such as Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[<span data-ttu-id="29f33-113">Muiden kuin selain sovellusten, jotka eivät voi kirja utua Office 365-, Azure-tai Intune-sovellukseen, vian määritys</span><span class="sxs-lookup"><span data-stu-id="29f33-113">How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune</span></span>](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[<span data-ttu-id="29f33-114">Office-tunniste tietoja pyydetään toistuvasti</span><span class="sxs-lookup"><span data-stu-id="29f33-114">Repeatedly prompted for credentials in Office</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)