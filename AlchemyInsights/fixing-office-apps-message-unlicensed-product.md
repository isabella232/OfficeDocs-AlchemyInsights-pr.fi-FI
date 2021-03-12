---
title: Officen aktivointi epäonnistui
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 3a42c221047e7be6a173694cd45136baa6bff39a
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704927"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="1a94a-102">Officen aktivointi epäonnistui</span><span class="sxs-lookup"><span data-stu-id="1a94a-102">Unable to activate Office</span></span>

- <span data-ttu-id="1a94a-103">Tarkista, onko tilauksesi vanhentunut.</span><span class="sxs-lookup"><span data-stu-id="1a94a-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="1a94a-104">Varmista, että käyttöoikeutesi sallii asiakaskäyttöoikeudet, kuten Office 365 Businessin tai Business Premiumin, ja että [käyttäjälle on määritetty käyttöoikeus](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="1a94a-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span></span>
- <span data-ttu-id="1a94a-105">Varmista, että käyttäjä kirjautuu Officeen tilillä, jolle on määritetty käyttöoikeus.</span><span class="sxs-lookup"><span data-stu-id="1a94a-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="1a94a-106">Tarkista [Office 365:n palvelun kunto -sivulla](https://docs.microsoft.com/office365/enterprise/view-service-health), onko palvelussa tunnettuja ongelmia.</span><span class="sxs-lookup"><span data-stu-id="1a94a-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="1a94a-107">Tarkista palomuurin, virustorjuntaohjelmiston ja välityspalvelimen asetukset ja varmista, etteivät ne estä Microsoft 365 -sovellusten yhteyttä Internetiin.</span><span class="sxs-lookup"><span data-stu-id="1a94a-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="1a94a-108">Lisätietoja on artikkelissa [Office 365:n URL-osoitteet ja IP-osoitealueet](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365:n URL-osoitteet ja IP-osoitealueet").</span><span class="sxs-lookup"><span data-stu-id="1a94a-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="1a94a-109">**Vihje** Voimme diagnosoida ja korjata useita Windows-tietokoneiden Officen yleisiä sisäänkirjautumisongelmia puolestasi automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="1a94a-109">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="1a94a-110">Jos haluat käyttää automaattista työkaluamme, lataa ja suorita **[Microsoftin tuki- ja palautusavustaja](https://aka.ms/SaRA-OfficeSignInScenario)**.</span><span class="sxs-lookup"><span data-stu-id="1a94a-110">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="1a94a-111">Tee vianmääritys seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="1a94a-111">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="1a94a-112">Avaa Office-sovellus ja [kirjaudu ulos](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) olemassa olevilta käyttäjätileiltä.</span><span class="sxs-lookup"><span data-stu-id="1a94a-112">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="1a94a-113">[Poista](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) ja [määritä uudelleen](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office-käyttöoikeus ja [kirjaudu sitten Officeen](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) käyttämällä kyseistä käyttäjätiliä.</span><span class="sxs-lookup"><span data-stu-id="1a94a-113">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="1a94a-114">[Aktivoinnin vianmääritysohjelman](https://aka.ms/SARA-OfficeActivation-Alchemy) suorittaminen</span><span class="sxs-lookup"><span data-stu-id="1a94a-114">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="1a94a-115">Officen aktivoinnin tilan palauttaminen</span><span class="sxs-lookup"><span data-stu-id="1a94a-115">Reset Office activation state</span></span>](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Officen aktivoinnin tilan palauttaminen")
- [<span data-ttu-id="1a94a-116">Officen online-korjauksen suorittaminen</span><span class="sxs-lookup"><span data-stu-id="1a94a-116">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="1a94a-117">Lisätietoja vianmäärityksestä on seuraavissa artikkeleissa:</span><span class="sxs-lookup"><span data-stu-id="1a94a-117">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="1a94a-118">Ei käyttöoikeutta -virheet ja aktivointivirheet Officessa</span><span class="sxs-lookup"><span data-stu-id="1a94a-118">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="1a94a-119">”Emme voi muodostaa yhteyttä tiliisi. Yritä myöhemmin uudelleen" -virhe Officen aktivoinnin yhteydessä</span><span class="sxs-lookup"><span data-stu-id="1a94a-119">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)