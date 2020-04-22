---
title: Office-sovellusten korjaaminen Valitettavasti meillä on tilapäispalvelinongelmien sanoma
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764114"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="559bb-102">Office-sovellusten korjaaminen "Anteeksi, meillä on tilapäisiä palvelinongelmia" -sanoma</span><span class="sxs-lookup"><span data-stu-id="559bb-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="559bb-103">Jos saat tämän sanoman, kokeile seuraavaa:</span><span class="sxs-lookup"><span data-stu-id="559bb-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="559bb-104">Tarkista palomuurin, virustentorjuntaohjelmiston ja välityspalvelimen asetukset ja varmista, että ne eivät estä Office-sovellusten Internet-yhteyttä.</span><span class="sxs-lookup"><span data-stu-id="559bb-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="559bb-105">Katso [URL-osoitteet ja IP-osoitealueet](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="559bb-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="559bb-106">Siirry **Käynnistä-kohtaan** > **Run**ja kirjoita **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="559bb-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="559bb-107">Varmista, että seuraavat palvelut ovat käynnissä:</span><span class="sxs-lookup"><span data-stu-id="559bb-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="559bb-108">Verkkoon liitettyjen laitteiden automaattinen asennus</span><span class="sxs-lookup"><span data-stu-id="559bb-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="559bb-109">Verkkoluettelopalvelu</span><span class="sxs-lookup"><span data-stu-id="559bb-109">Network List Service</span></span>
    - <span data-ttu-id="559bb-110">Verkon sijaintitietoisuus</span><span class="sxs-lookup"><span data-stu-id="559bb-110">Network Location Awareness</span></span>
    - <span data-ttu-id="559bb-111">Windowsin tapahtumaloki</span><span class="sxs-lookup"><span data-stu-id="559bb-111">Windows Event Log</span></span>

<span data-ttu-id="559bb-112">Jos jokin näistä palveluista ei ole käynnissä, yritä käynnistää se.</span><span class="sxs-lookup"><span data-stu-id="559bb-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="559bb-113">Jos palvelun käynnistämisessä on ongelmia, suorita seuraava komento avaamalla komentorivi, jolla on laajennetut käyttöoikeudet:</span><span class="sxs-lookup"><span data-stu-id="559bb-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="559bb-114">**Kävi koulua sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="559bb-114">**sfc /scannow**</span></span>

<span data-ttu-id="559bb-115">Kun tämä komento on valmis, käynnistä tietokone uudelleen.</span><span class="sxs-lookup"><span data-stu-id="559bb-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="559bb-116">Lisätietoja on kohdassa ["Valitettavasti emme voi muodostaa yhteyttä tiliisi. Yritä myöhemmin uudelleen" -virhe aktivoitaessa.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="559bb-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>