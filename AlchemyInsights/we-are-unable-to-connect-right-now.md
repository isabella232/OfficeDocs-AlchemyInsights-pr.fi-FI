---
title: Aktivointiongelma - Emme pysty muodostamaan yhteyttä juuri nyt
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581872"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="dce6d-102">Microsoft 365 -sovellusten "Emme pysty muodostamaan yhteyttä juuri nyt" -sanoman korjaaminen</span><span class="sxs-lookup"><span data-stu-id="dce6d-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="dce6d-103">Jos näyttöön tulee tämä sanoma, kokeile seuraavaa:</span><span class="sxs-lookup"><span data-stu-id="dce6d-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="dce6d-104">Tarkista palomuurin, virustentorjuntaohjelmiston ja välityspalvelimen asetukset ja varmista, että ne eivät estä Microsoft 365 -sovellusten Internet-käyttöä.</span><span class="sxs-lookup"><span data-stu-id="dce6d-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="dce6d-105">Lisätietoja [on kohdassa Microsoftin URL-osoitteet ja IP-osoitealueet](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="dce6d-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="dce6d-106">Siirry **Käynnistä**  >  **Suorita**ja kirjoita **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="dce6d-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="dce6d-107">Varmista, että kaikki seuraavat palvelut ovat käynnissä:</span><span class="sxs-lookup"><span data-stu-id="dce6d-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="dce6d-108">Verkkoon liitettyjen laitteiden automaattinen asennus</span><span class="sxs-lookup"><span data-stu-id="dce6d-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="dce6d-109">Verkkoluettelopalvelu</span><span class="sxs-lookup"><span data-stu-id="dce6d-109">Network List Service</span></span>
    - <span data-ttu-id="dce6d-110">Verkon sijainnin tunnettuus</span><span class="sxs-lookup"><span data-stu-id="dce6d-110">Network Location Awareness</span></span>
    - <span data-ttu-id="dce6d-111">Windowsin tapahtumaloki</span><span class="sxs-lookup"><span data-stu-id="dce6d-111">Windows Event Log</span></span>

<span data-ttu-id="dce6d-112">Jos jokin näistä palveluista ei ole käynnissä, yritä käynnistää se.</span><span class="sxs-lookup"><span data-stu-id="dce6d-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="dce6d-113">Jos palvelun käynnistämisessä on ongelmia, suorita seuraava komento avaamalla komentorivi, jolla on laajennetut käyttöoikeudet:</span><span class="sxs-lookup"><span data-stu-id="dce6d-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="dce6d-114">**sfc / scannow**</span><span class="sxs-lookup"><span data-stu-id="dce6d-114">**sfc /scannow**</span></span>

<span data-ttu-id="dce6d-115">Kun tämä komento on valmis, käynnistä tietokone uudelleen.</span><span class="sxs-lookup"><span data-stu-id="dce6d-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="dce6d-116">Lisätietoja on [ohjeaiheessa "Emme voi muodostaa yhteyttä tiliisi. Yritä myöhemmin uudelleen -virhe, kun aktivoit Officen Microsoft 365:stä.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="dce6d-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>