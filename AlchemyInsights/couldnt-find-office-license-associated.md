---
title: Microsoft 365 -sovellusten asentaminen ei löytänyt Office-käyttöoikeuksiin liittyvää viestiä
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
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816485"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="ce609-102">Microsoft 365 -sovellusten "Office-käyttöoikeuksia ei löytyi" -viestin asentaminen</span><span class="sxs-lookup"><span data-stu-id="ce609-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="ce609-103">Jos näyttöön tulee tämä sanoma, kokeile seuraavaa:</span><span class="sxs-lookup"><span data-stu-id="ce609-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="ce609-104">Tarkista palomuurin, virustentorjuntaohjelman ja välityspalvelimen asetukset ja varmista, että ne eivät estä Microsoft 365 -sovellusten Internet-yhteyttä.</span><span class="sxs-lookup"><span data-stu-id="ce609-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="ce609-105">Katso [Microsoft 365:n URL-osoitteet ja IP-osoitealueet.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="ce609-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="ce609-106">Poista ja [varaa uudelleen Office-käyttöoikeus käyttäjälle,](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) jota ongelma koskee.</span><span class="sxs-lookup"><span data-stu-id="ce609-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="ce609-107">Avaa Office-sovellus ja [kirjaudu ulos](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) olemassa olevista käyttäjätileistä.</span><span class="sxs-lookup"><span data-stu-id="ce609-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="ce609-108">Siirry kohtaan Windowsin asetukset >  >  **Sähköpostitilit & tilit** ja poista kaikki työtilit paitsi kyseinen tili.</span><span class="sxs-lookup"><span data-stu-id="ce609-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="ce609-109">Siirry kohtaan Windowsin asetukset >  >  **Tilit Käytä työtä tai koulua** ja katkaise kaikkien työtilien yhteys, paitsi kyseinen tili.</span><span class="sxs-lookup"><span data-stu-id="ce609-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="ce609-110">Palauta Officen aktivoinnin tila.</span><span class="sxs-lookup"><span data-stu-id="ce609-110">Reset the Office activation state.</span></span> <span data-ttu-id="ce609-111">[Ohjeet](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="ce609-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="ce609-112">[Kirjaudu sisään](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) käyttämällä käyttäjätiliä, jota ongelma koskee.</span><span class="sxs-lookup"><span data-stu-id="ce609-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="ce609-113">Katso lisää vianmääritysratkaisuja ohjeista [Ei käyttöomistajaa ja aktivointivirheitä Officessa.](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="ce609-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>