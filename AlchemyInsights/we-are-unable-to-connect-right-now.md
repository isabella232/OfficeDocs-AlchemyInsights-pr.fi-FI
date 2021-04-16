---
title: Aktivointiongelma – Yhteyttä ei voida muodostaa juuri nyt
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
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806439"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="4eb54-102">Microsoft 365 -sovellusten "Yhteyttä ei voida juuri nyt" -viestin asentaminen</span><span class="sxs-lookup"><span data-stu-id="4eb54-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="4eb54-103">Jos näyttöön tulee tämä sanoma, kokeile seuraavaa:</span><span class="sxs-lookup"><span data-stu-id="4eb54-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="4eb54-104">Tarkista palomuurin, virustentorjuntaohjelman ja välityspalvelimen asetukset ja varmista, että ne eivät estä Microsoft 365 -sovellusten Internet-yhteyttä.</span><span class="sxs-lookup"><span data-stu-id="4eb54-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="4eb54-105">Katso [Microsoftin URL-osoitteet ja IP-osoitealueet.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="4eb54-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="4eb54-106">Siirry Käynnistä **Suorita**  >  **-valikkoon** ja kirjoita **services.msc.**</span><span class="sxs-lookup"><span data-stu-id="4eb54-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="4eb54-107">Varmista, että seuraavat palvelut ovat käynnissä:</span><span class="sxs-lookup"><span data-stu-id="4eb54-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="4eb54-108">Verkkoon yhdistetyt laitteet – automaattinen määritys</span><span class="sxs-lookup"><span data-stu-id="4eb54-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="4eb54-109">Verkkoluettelopalvelu</span><span class="sxs-lookup"><span data-stu-id="4eb54-109">Network List Service</span></span>
    - <span data-ttu-id="4eb54-110">Verkkosijainnin tietoisuus</span><span class="sxs-lookup"><span data-stu-id="4eb54-110">Network Location Awareness</span></span>
    - <span data-ttu-id="4eb54-111">Windowsin tapahtumaloki</span><span class="sxs-lookup"><span data-stu-id="4eb54-111">Windows Event Log</span></span>

<span data-ttu-id="4eb54-112">Jos jokin näistä palveluista ei ole käynnissä, yritä käynnistää se.</span><span class="sxs-lookup"><span data-stu-id="4eb54-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="4eb54-113">Jos palvelun avaamisessa ilmenee ongelmia, suorita seuraava komento avaamalla komentokehote, jossa on järjestelmänvalvojan oikeudet:</span><span class="sxs-lookup"><span data-stu-id="4eb54-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="4eb54-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="4eb54-114">**sfc /scannow**</span></span>

<span data-ttu-id="4eb54-115">Kun tämä komento on valmis, käynnistä tietokone uudelleen.</span><span class="sxs-lookup"><span data-stu-id="4eb54-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="4eb54-116">Lisätietoja on [kohdassa "Tiliisi ei voi muodostaa yhteyttä. Yritä myöhemmin uudelleen"-virhe aktivoitaessa Officen Microsoft 365:stä.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="4eb54-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>