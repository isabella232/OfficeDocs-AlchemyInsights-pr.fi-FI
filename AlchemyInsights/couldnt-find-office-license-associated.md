---
title: Microsoft 365 -sovellusten korjaaminen Office-käyttöoikeuksille ei löytynyt viestiä
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
ms.openlocfilehash: 65ffae1a784f841cb08a5df52b02671a4526d9d4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580438"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="a25e1-102">Microsoft 365 -sovellusten "Office-käyttöoikeuksia ei löytynyt" -sanoman korjaaminen</span><span class="sxs-lookup"><span data-stu-id="a25e1-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="a25e1-103">Jos näyttöön tulee tämä sanoma, kokeile seuraavaa:</span><span class="sxs-lookup"><span data-stu-id="a25e1-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="a25e1-104">Tarkista palomuurin, virustentorjuntaohjelmiston ja välityspalvelimen asetukset ja varmista, että ne eivät estä Microsoft 365 -sovellusten Internet-käyttöä.</span><span class="sxs-lookup"><span data-stu-id="a25e1-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="a25e1-105">Lisätietoja on [microsoft 365:n URL-osoitteissa ja IP-osoitealueissa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="a25e1-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="a25e1-106">Poista [Office-käyttöoikeus](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ja määritä se uudelleen haavoittuvuuden sisältävälle käyttäjälle.</span><span class="sxs-lookup"><span data-stu-id="a25e1-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="a25e1-107">Avaa Office-sovellus ja [kirjaudu ulos](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) olemassa olevista käyttäjätileistä.</span><span class="sxs-lookup"><span data-stu-id="a25e1-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="a25e1-108">Siirry Windowsin asetukset > **Tilit**  >  **Sähköposti & -tileille**ja poista kaikki työtilit kyseistä tiliä lukuun ottamatta.</span><span class="sxs-lookup"><span data-stu-id="a25e1-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="a25e1-109">Siirry Windowsin asetukset > **Tilit**  >  **Accessin työpaikan tai oppilaitoksen**käyttöön ja katkaise kaikkien työtilien yhteys lukuun ottamatta tiliä, jota haavoittuvuus koskee.</span><span class="sxs-lookup"><span data-stu-id="a25e1-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="a25e1-110">Palauta Officen aktivoinnin tila.</span><span class="sxs-lookup"><span data-stu-id="a25e1-110">Reset the Office activation state.</span></span> <span data-ttu-id="a25e1-111">[Ohjeet](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="a25e1-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="a25e1-112">[Kirjaudu sisään](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) käyttämällä kyseistä käyttäjätiliä.</span><span class="sxs-lookup"><span data-stu-id="a25e1-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="a25e1-113">Lisätietoja vianmäärityksestä on artikkelissa [Käyttöoikeudeton tuote- ja aktivointivirheet Officessa](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="a25e1-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>