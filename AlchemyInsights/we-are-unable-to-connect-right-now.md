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
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716169"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="f7c0f-102">Office-sovellusten korjaaminen "Emme pysty muodostamaan yhteyttä juuri nyt" -sanoma</span><span class="sxs-lookup"><span data-stu-id="f7c0f-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="f7c0f-103">Jos saat tämän sanoman, kokeile seuraavaa:</span><span class="sxs-lookup"><span data-stu-id="f7c0f-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="f7c0f-104">Tarkista palomuurin, virustentorjuntaohjelmiston ja välityspalvelimen asetukset ja varmista, että ne eivät estä Office-sovellusten Internet-yhteyttä.</span><span class="sxs-lookup"><span data-stu-id="f7c0f-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="f7c0f-105">Lisätietoja on [ohjeaiheessa Microsoftin URL-osoitteet ja IP-osoitealueet](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="f7c0f-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="f7c0f-106">Siirry **Käynnistä-kohtaan** > **Run**ja kirjoita **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="f7c0f-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="f7c0f-107">Varmista, että seuraavat palvelut ovat käynnissä:</span><span class="sxs-lookup"><span data-stu-id="f7c0f-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="f7c0f-108">Verkkoon liitettyjen laitteiden automaattinen asennus</span><span class="sxs-lookup"><span data-stu-id="f7c0f-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="f7c0f-109">Verkkoluettelopalvelu</span><span class="sxs-lookup"><span data-stu-id="f7c0f-109">Network List Service</span></span>
    - <span data-ttu-id="f7c0f-110">Verkon sijaintitietoisuus</span><span class="sxs-lookup"><span data-stu-id="f7c0f-110">Network Location Awareness</span></span>
    - <span data-ttu-id="f7c0f-111">Windowsin tapahtumaloki</span><span class="sxs-lookup"><span data-stu-id="f7c0f-111">Windows Event Log</span></span>

<span data-ttu-id="f7c0f-112">Jos jokin näistä palveluista ei ole käynnissä, yritä käynnistää se.</span><span class="sxs-lookup"><span data-stu-id="f7c0f-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="f7c0f-113">Jos palvelun käynnistämisessä on ongelmia, suorita seuraava komento avaamalla komentorivi, jolla on laajennetut käyttöoikeudet:</span><span class="sxs-lookup"><span data-stu-id="f7c0f-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="f7c0f-114">**Kävi koulua sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="f7c0f-114">**sfc /scannow**</span></span>

<span data-ttu-id="f7c0f-115">Kun tämä komento on valmis, käynnistä tietokone uudelleen.</span><span class="sxs-lookup"><span data-stu-id="f7c0f-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="f7c0f-116">Lisätietoja on kohdassa ["Valitettavasti emme voi muodostaa yhteyttä tiliisi. Yritä myöhemmin uudelleen" -virhe, kun aktivoit Officen Microsoft 365:stä.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="f7c0f-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>