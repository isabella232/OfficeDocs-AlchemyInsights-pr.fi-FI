---
title: Lisensoimattomien tuotevirheiden ratkaiseminen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: 89d0e589329d40f17c36baa54868154be0f5b887
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582736"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a><span data-ttu-id="e2827-102">Ehdotuksia luvattoman tuotteen virheiden ratkaisemiseksi</span><span class="sxs-lookup"><span data-stu-id="e2827-102">Suggestions for solving "Unlicensed Product" errors</span></span>

<span data-ttu-id="e2827-103">Voit ratkaista "Lisensoimaton tuote" -virheitä seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="e2827-103">To solve errors about an "Unlicensed Product," try the following:</span></span>

- <span data-ttu-id="e2827-104">Tarkista, onko tilauksesi tila vanhentunut.</span><span class="sxs-lookup"><span data-stu-id="e2827-104">Check to see if your subscription status has expired.</span></span>
- <span data-ttu-id="e2827-105">Varmista, että sinulla on tilaus, joka sallii asiakaskäyttöoikeudet, kuten Microsoft 365 Apps for Business tai Business Premium, ja [varmista, että käyttäjälle on määritetty käyttöoikeus.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="e2827-105">Make sure you have a subscription that allows client licenses, such as Microsoft 365 Apps for business or Business Premium, and [ensure that the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> 
- <span data-ttu-id="e2827-106">Varmista, että käyttäjä on kirjautuu Officeen samalla tilillä, jolle on määritetty käyttöoikeus.</span><span class="sxs-lookup"><span data-stu-id="e2827-106">Make sure the user is signing in to Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="e2827-107">Tarkista [Palvelun kunto -sivulta,](https://docs.microsoft.com/office365/enterprise/view-service-health) onko palvelussa tunnettuja ongelmia.</span><span class="sxs-lookup"><span data-stu-id="e2827-107">Check the [Service health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="e2827-108">Tarkista palomuurin, virustentorjuntaohjelmiston ja välityspalvelimen asetukset ja varmista, että ne eivät estä Microsoft 365 -sovellusten Internet-käyttöä.</span><span class="sxs-lookup"><span data-stu-id="e2827-108">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the Internet.</span></span> <span data-ttu-id="e2827-109">Katso [URL-osoitteet ja IP-osoitealueet](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="e2827-109">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

<span data-ttu-id="e2827-110">Voit myös kokeilla seuraavia vianmääritystoimia:</span><span class="sxs-lookup"><span data-stu-id="e2827-110">You may also try the following troubleshooting actions:</span></span> 

- <span data-ttu-id="e2827-111">Avaa Office-sovellus ja [kirjaudu ulos](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) olemassa olevista käyttäjätileistä.</span><span class="sxs-lookup"><span data-stu-id="e2827-111">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="e2827-112">[Poista](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) [Office-käyttöoikeus](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ja määritä se uudelleen ja kirjaudu sitten [Officeen](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) käyttämällä kyseistä käyttäjätiliä.</span><span class="sxs-lookup"><span data-stu-id="e2827-112">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) the Office license, and then [sign in to Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="e2827-113">Suorita [aktivoinnin vianmääritys](https://aka.ms/SARA-OfficeActivation-Alchemy).</span><span class="sxs-lookup"><span data-stu-id="e2827-113">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy).</span></span>
- <span data-ttu-id="e2827-114">[Palauta Officen aktivoinnin tila](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="e2827-114">[Reset the Office activation state](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span> 
- <span data-ttu-id="e2827-115">[Officen online-korjauksen suorittaminen](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span><span class="sxs-lookup"><span data-stu-id="e2827-115">[Perform an Online Repair of Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span></span>

<span data-ttu-id="e2827-116">Lisätietoja vianmäärityksestä on seuraavissa artikkeleissa:</span><span class="sxs-lookup"><span data-stu-id="e2827-116">For additional troubleshooting solutions, see:</span></span> 

- [<span data-ttu-id="e2827-117">Ei käyttöoikeutta -virheet ja aktivointivirheet Officessa</span><span class="sxs-lookup"><span data-stu-id="e2827-117">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [<span data-ttu-id="e2827-118">”Emme voi muodostaa yhteyttä tiliisi. Yritä myöhemmin uudelleen" -virhe Officen aktivoinnin yhteydessä</span><span class="sxs-lookup"><span data-stu-id="e2827-118">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)