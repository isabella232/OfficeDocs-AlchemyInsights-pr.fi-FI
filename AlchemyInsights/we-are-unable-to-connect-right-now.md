---
title: Aktivointi ongelma-emme voi muodostaa yhteyttä juuri nyt
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
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628239"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="2981d-102">Office-sovellusten korjaaminen "emme pysty yhdistämään juuri nyt"-viestiä</span><span class="sxs-lookup"><span data-stu-id="2981d-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="2981d-103">Jos tämä sanoma tulee näyttöön, kokeile seuraavia:</span><span class="sxs-lookup"><span data-stu-id="2981d-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="2981d-104">Tarkista palo muuri-, virustentorjuntaohjelmisto-ja välitys palvelin asetukset ja varmista, etteivät ne estä Internet-pääsyä Office-sovelluksiin.</span><span class="sxs-lookup"><span data-stu-id="2981d-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="2981d-105">Katso [Office 365-URL-osoitteet ja IP-osoite alueet](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="2981d-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="2981d-106">Siirry kohtaan **Aloita** > **suorittaminen**ja kirjoita **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="2981d-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="2981d-107">Varmista, että seuraavat palvelut ovat käynnissä:</span><span class="sxs-lookup"><span data-stu-id="2981d-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="2981d-108">Verkkoon liitettyjen laitteiden automaattinen määritys</span><span class="sxs-lookup"><span data-stu-id="2981d-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="2981d-109">Verkko luettelo palvelu</span><span class="sxs-lookup"><span data-stu-id="2981d-109">Network List Service</span></span>
    - <span data-ttu-id="2981d-110">Verkon sijainti tietoisuus</span><span class="sxs-lookup"><span data-stu-id="2981d-110">Network Location Awareness</span></span>
    - <span data-ttu-id="2981d-111">Windowsin tapahtuma loki</span><span class="sxs-lookup"><span data-stu-id="2981d-111">Windows Event Log</span></span>

<span data-ttu-id="2981d-112">Jos jokin näistä palveluista ei ole käynnissä, yritä käynnistää se.</span><span class="sxs-lookup"><span data-stu-id="2981d-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="2981d-113">Jos sinulla on ongelmia palvelun käynnistettäessä, suorita seuraava komento avaamalla komento kehote, jossa on laajennettuja käyttö oikeuksia:</span><span class="sxs-lookup"><span data-stu-id="2981d-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="2981d-114">**SFC/scannow**</span><span class="sxs-lookup"><span data-stu-id="2981d-114">**sfc /scannow**</span></span>

<span data-ttu-id="2981d-115">Kun tämä komento on suoritettu, Käynnistä tieto kone uudelleen.</span><span class="sxs-lookup"><span data-stu-id="2981d-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="2981d-116">Lisä tietoja on kohdassa ["anteeksi, emme voi muodostaa yhteyttä tiliisi. Yritä myöhemmin uudelleen "-virhe, kun Akti voit Officen Office-365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="2981d-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>