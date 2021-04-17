---
title: Microsoft 365 -sovellusten asentaminen Valitettavasti Tilapäiset palvelinongelmat -viesti
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
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835268"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="f8ba5-102">Microsoft 365 -sovellusten "Tilapäiset palvelinongelmat valitettavasti" -viestin asentaminen</span><span class="sxs-lookup"><span data-stu-id="f8ba5-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="f8ba5-103">Jos näyttöön tulee tämä sanoma, kokeile seuraavaa:</span><span class="sxs-lookup"><span data-stu-id="f8ba5-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="f8ba5-104">Tarkista palomuurin, virustentorjuntaohjelman ja välityspalvelimen asetukset ja varmista, että ne eivät estä Microsoft 365 -sovellusten Internet-yhteyttä.</span><span class="sxs-lookup"><span data-stu-id="f8ba5-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="f8ba5-105">Katso [URL-osoitteet ja IP-osoitealueet.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="f8ba5-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="f8ba5-106">Siirry Käynnistä **Suorita**  >  **-valikkoon** ja kirjoita **services.msc.**</span><span class="sxs-lookup"><span data-stu-id="f8ba5-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="f8ba5-107">Varmista, että seuraavat palvelut ovat käynnissä:</span><span class="sxs-lookup"><span data-stu-id="f8ba5-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="f8ba5-108">Verkkoon yhdistetyt laitteet – automaattinen määritys</span><span class="sxs-lookup"><span data-stu-id="f8ba5-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="f8ba5-109">Verkkoluettelopalvelu</span><span class="sxs-lookup"><span data-stu-id="f8ba5-109">Network List Service</span></span>
    - <span data-ttu-id="f8ba5-110">Verkkosijainnin tietoisuus</span><span class="sxs-lookup"><span data-stu-id="f8ba5-110">Network Location Awareness</span></span>
    - <span data-ttu-id="f8ba5-111">Windowsin tapahtumaloki</span><span class="sxs-lookup"><span data-stu-id="f8ba5-111">Windows Event Log</span></span>

<span data-ttu-id="f8ba5-112">Jos jokin näistä palveluista ei ole käynnissä, yritä käynnistää se.</span><span class="sxs-lookup"><span data-stu-id="f8ba5-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="f8ba5-113">Jos palvelun avaamisessa ilmenee ongelmia, suorita seuraava komento avaamalla komentokehote, jossa on järjestelmänvalvojan oikeudet:</span><span class="sxs-lookup"><span data-stu-id="f8ba5-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="f8ba5-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="f8ba5-114">**sfc /scannow**</span></span>

<span data-ttu-id="f8ba5-115">Kun tämä komento on valmis, käynnistä tietokone uudelleen.</span><span class="sxs-lookup"><span data-stu-id="f8ba5-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="f8ba5-116">Lisätietoja on [kohdassa "Tiliisi ei voi muodostaa yhteyttä. Yritä myöhemmin uudelleen"-virhe aktivoitaessa](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="f8ba5-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>