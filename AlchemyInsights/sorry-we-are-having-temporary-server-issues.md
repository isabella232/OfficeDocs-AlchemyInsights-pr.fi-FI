---
title: Fixing Microsoft 365-sovellukset Pahoittelemme, meillä on väliaikainen palvelin ongelmien viesti
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
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758242"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="a6455-102">Microsoft 365-sovellusten korjaaminen "Valitettavasti meillä on väliaikaisia palvelin ongelmia"-viesti</span><span class="sxs-lookup"><span data-stu-id="a6455-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="a6455-103">Jos saat tämän viestin, kokeile seuraavaa:</span><span class="sxs-lookup"><span data-stu-id="a6455-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="a6455-104">Tarkista palo muurin, virustentorjuntaohjelman ja välitys palvelimen asetukset ja varmista, että ne eivät estä Internet-yhteyttä Microsoft 365-sovelluksiin.</span><span class="sxs-lookup"><span data-stu-id="a6455-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="a6455-105">Katso [URL-osoitteet ja IP-osoite alueet](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="a6455-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="a6455-106">Siirry **Käynnistä**  >  **Suorita**-kohtaan ja kirjoita **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="a6455-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="a6455-107">Varmista, että seuraavat palvelut ovat käynnissä:</span><span class="sxs-lookup"><span data-stu-id="a6455-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="a6455-108">Verkkoon yhdistetyt laitteet automaattinen määritys</span><span class="sxs-lookup"><span data-stu-id="a6455-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="a6455-109">Verkko luettelon palvelu</span><span class="sxs-lookup"><span data-stu-id="a6455-109">Network List Service</span></span>
    - <span data-ttu-id="a6455-110">Verkko sijainnin tietoisuus</span><span class="sxs-lookup"><span data-stu-id="a6455-110">Network Location Awareness</span></span>
    - <span data-ttu-id="a6455-111">Windowsin tapahtuma loki</span><span class="sxs-lookup"><span data-stu-id="a6455-111">Windows Event Log</span></span>

<span data-ttu-id="a6455-112">Jos jokin näistä palveluista ei ole käynnissä, yritä käynnistää se.</span><span class="sxs-lookup"><span data-stu-id="a6455-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="a6455-113">Jos sinulla on ongelmia palvelun aloittamisessa, suorita seuraava komento avaamalla komento kehote laajenne tuilla käyttö oikeuksilla:</span><span class="sxs-lookup"><span data-stu-id="a6455-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="a6455-114">**SFC/scannow**</span><span class="sxs-lookup"><span data-stu-id="a6455-114">**sfc /scannow**</span></span>

<span data-ttu-id="a6455-115">Kun tämä komento on valmis, Käynnistä tieto kone uudelleen.</span><span class="sxs-lookup"><span data-stu-id="a6455-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="a6455-116">Katso lisä tietoja kohdasta ["Pahoittelemme, emme voi muodostaa yhteyttä tiliisi. Yritä myöhemmin uudelleen-virhe aktivoitaessa](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="a6455-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>