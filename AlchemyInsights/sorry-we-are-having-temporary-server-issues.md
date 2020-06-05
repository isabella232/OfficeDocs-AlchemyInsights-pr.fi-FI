---
title: Microsoft 365 -sovellusten korjaaminen Anteeksi, meillä on tilapäisiä palvelinongelmia -sanoma
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
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582700"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="66b55-102">Microsoft 365 -sovellusten korjaaminen "Anteeksi, meillä on tilapäisiä palvelinongelmia" -sanoma</span><span class="sxs-lookup"><span data-stu-id="66b55-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="66b55-103">Jos näyttöön tulee tämä sanoma, kokeile seuraavaa:</span><span class="sxs-lookup"><span data-stu-id="66b55-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="66b55-104">Tarkista palomuurin, virustentorjuntaohjelmiston ja välityspalvelimen asetukset ja varmista, että ne eivät estä Microsoft 365 -sovellusten Internet-käyttöä.</span><span class="sxs-lookup"><span data-stu-id="66b55-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="66b55-105">Katso [URL-osoitteet ja IP-osoitealueet](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="66b55-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="66b55-106">Siirry **Käynnistä**  >  **Suorita**ja kirjoita **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="66b55-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="66b55-107">Varmista, että kaikki seuraavat palvelut ovat käynnissä:</span><span class="sxs-lookup"><span data-stu-id="66b55-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="66b55-108">Verkkoon liitettyjen laitteiden automaattinen asennus</span><span class="sxs-lookup"><span data-stu-id="66b55-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="66b55-109">Verkkoluettelopalvelu</span><span class="sxs-lookup"><span data-stu-id="66b55-109">Network List Service</span></span>
    - <span data-ttu-id="66b55-110">Verkon sijainnin tunnettuus</span><span class="sxs-lookup"><span data-stu-id="66b55-110">Network Location Awareness</span></span>
    - <span data-ttu-id="66b55-111">Windowsin tapahtumaloki</span><span class="sxs-lookup"><span data-stu-id="66b55-111">Windows Event Log</span></span>

<span data-ttu-id="66b55-112">Jos jokin näistä palveluista ei ole käynnissä, yritä käynnistää se.</span><span class="sxs-lookup"><span data-stu-id="66b55-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="66b55-113">Jos palvelun käynnistämisessä on ongelmia, suorita seuraava komento avaamalla komentorivi, jolla on laajennetut käyttöoikeudet:</span><span class="sxs-lookup"><span data-stu-id="66b55-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="66b55-114">**sfc / scannow**</span><span class="sxs-lookup"><span data-stu-id="66b55-114">**sfc /scannow**</span></span>

<span data-ttu-id="66b55-115">Kun tämä komento on valmis, käynnistä tietokone uudelleen.</span><span class="sxs-lookup"><span data-stu-id="66b55-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="66b55-116">Lisätietoja on [ohjeaiheessa "Emme voi muodostaa yhteyttä tiliisi. Yritä myöhemmin uudelleen -virhe, kun aktivoit](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="66b55-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>