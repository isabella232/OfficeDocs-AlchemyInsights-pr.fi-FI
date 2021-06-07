---
title: Officen aktivointi epäonnistui
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798677"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="98d97-102">Officen aktivointi epäonnistui</span><span class="sxs-lookup"><span data-stu-id="98d97-102">Unable to activate Office</span></span>

<span data-ttu-id="98d97-103">**Huomautus:** Jos käytät vanhempaa Windows (esimerkiksi Windows 7), varmista, että TLS 1.2 on käytössä oletusversiona.</span><span class="sxs-lookup"><span data-stu-id="98d97-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="98d97-104">Lisätietoja on päivityksessä [TLS 1.1: n ja TLS 1.2:n käyttöönottamiseksi WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392):n oletusarvoina suojattuina protokollina.</span><span class="sxs-lookup"><span data-stu-id="98d97-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="98d97-105">Tarkista, onko tilauksesi vanhentunut.</span><span class="sxs-lookup"><span data-stu-id="98d97-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="98d97-106">Varmista, että käyttöoikeutesi sallii asiakaskäyttöoikeudet, kuten Office 365 Businessin tai Business Premiumin, ja että [käyttäjälle on määritetty käyttöoikeus](/microsoft-365/admin/manage/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="98d97-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="98d97-107">Varmista, että käyttäjä kirjautuu Officeen tilillä, jolle on määritetty käyttöoikeus.</span><span class="sxs-lookup"><span data-stu-id="98d97-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="98d97-108">Tarkista [Office 365:n palvelun kunto -sivulla](/office365/enterprise/view-service-health), onko palvelussa tunnettuja ongelmia.</span><span class="sxs-lookup"><span data-stu-id="98d97-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="98d97-109">Tarkista palomuurin, virustorjuntaohjelmiston ja välityspalvelimen asetukset ja varmista, etteivät ne estä Microsoft 365 -sovellusten yhteyttä Internetiin.</span><span class="sxs-lookup"><span data-stu-id="98d97-109">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="98d97-110">Lisätietoja on artikkelissa [Office 365:n URL-osoitteet ja IP-osoitealueet](/office365/enterprise/urls-and-ip-address-ranges "Office 365:n URL-osoitteet ja IP-osoitealueet").</span><span class="sxs-lookup"><span data-stu-id="98d97-110">Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="98d97-111">**Vihje** Voimme diagnosoida ja korjata useita Windows-tietokoneiden Officen yleisiä sisäänkirjautumisongelmia puolestasi automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="98d97-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="98d97-112">Jos haluat käyttää automaattista työkaluamme, lataa ja suorita **[Microsoftin tuki- ja palautusavustaja](https://aka.ms/SaRA-OfficeSignInScenario)**.</span><span class="sxs-lookup"><span data-stu-id="98d97-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="98d97-113">Tee vianmääritys seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="98d97-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="98d97-114">Avaa Office-sovellus ja [kirjaudu ulos](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) olemassa olevilta käyttäjätileiltä.</span><span class="sxs-lookup"><span data-stu-id="98d97-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="98d97-115">[Poista](/microsoft-365/admin/manage/remove-licenses-from-users) ja [määritä uudelleen](/microsoft-365/admin/manage/assign-licenses-to-users) Office-käyttöoikeus ja [kirjaudu sitten Officeen](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) käyttämällä kyseistä käyttäjätiliä.</span><span class="sxs-lookup"><span data-stu-id="98d97-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="98d97-116">[Aktivoinnin vianmääritysohjelman](https://aka.ms/SARA-OfficeActivation-Alchemy) suorittaminen</span><span class="sxs-lookup"><span data-stu-id="98d97-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="98d97-117">Officen aktivoinnin tilan palauttaminen</span><span class="sxs-lookup"><span data-stu-id="98d97-117">Reset Office activation state</span></span>](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Officen aktivoinnin tilan palauttaminen")
- [<span data-ttu-id="98d97-118">Officen online-korjauksen suorittaminen</span><span class="sxs-lookup"><span data-stu-id="98d97-118">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="98d97-119">Lisätietoja vianmäärityksestä on seuraavissa artikkeleissa:</span><span class="sxs-lookup"><span data-stu-id="98d97-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="98d97-120">Ei käyttöoikeutta -virheet ja aktivointivirheet Officessa</span><span class="sxs-lookup"><span data-stu-id="98d97-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="98d97-121">”Emme voi muodostaa yhteyttä tiliisi. Yritä myöhemmin uudelleen" -virhe Officen aktivoinnin yhteydessä</span><span class="sxs-lookup"><span data-stu-id="98d97-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)