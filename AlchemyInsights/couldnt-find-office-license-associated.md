---
title: Office-sovellusten korjaaminen Office-käyttöoikeuteen liittyvää viestiä ei löytynyt
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 887be4bee2bd1562bdc3b29783e9deafe47d8d57
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505864"
---
# <a name="fixing-the-office-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="996d7-102">Office-sovellusten "Office-käyttöoikeuksia ei löytynyt" -sanoman korjaaminen</span><span class="sxs-lookup"><span data-stu-id="996d7-102">Fixing the Office apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="996d7-103">Jos näyttöön tulee tämä sanoma, kokeile seuraavaa:</span><span class="sxs-lookup"><span data-stu-id="996d7-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="996d7-104">Tarkista palomuurin, virustentorjuntaohjelmiston ja välityspalvelimen asetukset ja varmista, että ne eivät estä Office-sovellusten Internet-käyttöä.</span><span class="sxs-lookup"><span data-stu-id="996d7-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="996d7-105">Lisätietoja on [microsoft 365:n URL-osoitteissa ja IP-osoitealueissa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="996d7-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="996d7-106">Poista [Office-käyttöoikeus](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ja määritä se uudelleen haavoittuvuuden sisältävälle käyttäjälle.</span><span class="sxs-lookup"><span data-stu-id="996d7-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="996d7-107">Avaa Office-sovellus ja [kirjaudu ulos](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) olemassa olevista käyttäjätileistä.</span><span class="sxs-lookup"><span data-stu-id="996d7-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="996d7-108">Siirry Windowsin asetukset > **Tilit**  >  **Sähköposti & -tileille**ja poista kaikki työtilit kyseistä tiliä lukuun ottamatta.</span><span class="sxs-lookup"><span data-stu-id="996d7-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="996d7-109">Siirry Windowsin asetukset > **Tilit**  >  **Accessin työpaikan tai oppilaitoksen**käyttöön ja katkaise kaikkien työtilien yhteys lukuun ottamatta tiliä, jota haavoittuvuus koskee.</span><span class="sxs-lookup"><span data-stu-id="996d7-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="996d7-110">Palauta Officen aktivoinnin tila.</span><span class="sxs-lookup"><span data-stu-id="996d7-110">Reset the Office activation state.</span></span> <span data-ttu-id="996d7-111">[Ohjeet](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="996d7-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="996d7-112">[Kirjaudu sisään](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) käyttämällä kyseistä käyttäjätiliä.</span><span class="sxs-lookup"><span data-stu-id="996d7-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="996d7-113">Lisätietoja vianmäärityksestä on artikkelissa [Käyttöoikeudeton tuote- ja aktivointivirheet Officessa](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="996d7-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>