---
title: Lisensoimattomien tuote virheiden ratkaiseminen
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
- "3412"
- "9001428"
ms.openlocfilehash: bd2e8cb204edd7135fc34ef0d42ac8259434d37d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737950"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a><span data-ttu-id="d3ef6-102">Ehdotuksia "käyttöoikeudettoman tuotteen" virheiden ratkaisemiseksi</span><span class="sxs-lookup"><span data-stu-id="d3ef6-102">Suggestions for solving "Unlicensed Product" errors</span></span>

<span data-ttu-id="d3ef6-103">Jos haluat ratkaista Käyttöoikeudetonta tuotetta koskevia virheitä, kokeile seuraavaa:</span><span class="sxs-lookup"><span data-stu-id="d3ef6-103">To solve errors about an "Unlicensed Product," try the following:</span></span>

- <span data-ttu-id="d3ef6-104">Tarkista, onko tilauksesi tila vanhentunut.</span><span class="sxs-lookup"><span data-stu-id="d3ef6-104">Check to see if your subscription status has expired.</span></span>
- <span data-ttu-id="d3ef6-105">Varmista, että sinulla on tilaus, joka sallii asiakas käyttö oikeudet, kuten Microsoft 365-sovellukset Business-tai Business Premium-sovelluksessa, ja varmista, [että käyttäjälle on määritetty käyttö oikeus](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="d3ef6-105">Make sure you have a subscription that allows client licenses, such as Microsoft 365 Apps for business or Business Premium, and [ensure that the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> 
- <span data-ttu-id="d3ef6-106">Varmista, että käyttäjä on kirjautunut Officeen samalla tilillä, jolle käyttö oikeus on määritetty.</span><span class="sxs-lookup"><span data-stu-id="d3ef6-106">Make sure the user is signing in to Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="d3ef6-107">Tarkista [palvelun kunto-sivulla](https://docs.microsoft.com/office365/enterprise/view-service-health) , onko palvelussa tiedossa ongelmia.</span><span class="sxs-lookup"><span data-stu-id="d3ef6-107">Check the [Service health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="d3ef6-108">Tarkista palo muurin, virustentorjuntaohjelman ja välitys palvelimen asetukset ja varmista, että ne eivät estä Microsoft 365-sovelluksia, jotka käyttävät Internetiä.</span><span class="sxs-lookup"><span data-stu-id="d3ef6-108">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the Internet.</span></span> <span data-ttu-id="d3ef6-109">Katso [URL-osoitteet ja IP-osoite alueet](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="d3ef6-109">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

<span data-ttu-id="d3ef6-110">Voit myös kokeilla seuraavia vian määritys toimia:</span><span class="sxs-lookup"><span data-stu-id="d3ef6-110">You may also try the following troubleshooting actions:</span></span> 

- <span data-ttu-id="d3ef6-111">Avaa Office-sovellus ja [Kirjaudu ulos](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) olemassa olevista käyttäjä tileistäsi.</span><span class="sxs-lookup"><span data-stu-id="d3ef6-111">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="d3ef6-112">[Poista](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) Office-käyttö oikeus ja [Määritä se uudelleen](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ja [Kirjaudu sitten sisään Officeen](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) haavoittuvuuden sisältävän käyttäjä tilin avulla.</span><span class="sxs-lookup"><span data-stu-id="d3ef6-112">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) the Office license, and then [sign in to Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="d3ef6-113">Suorita [Akti voinnin vian määritys](https://aka.ms/SARA-OfficeActivation-Alchemy).</span><span class="sxs-lookup"><span data-stu-id="d3ef6-113">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy).</span></span>
- <span data-ttu-id="d3ef6-114">[Palauta Officen aktivoinnin tila](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="d3ef6-114">[Reset the Office activation state](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span> 
- <span data-ttu-id="d3ef6-115">[Suorita Officen online-korjaus](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span><span class="sxs-lookup"><span data-stu-id="d3ef6-115">[Perform an Online Repair of Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span></span>

<span data-ttu-id="d3ef6-116">Lisätietoja vianmäärityksestä on seuraavissa artikkeleissa:</span><span class="sxs-lookup"><span data-stu-id="d3ef6-116">For additional troubleshooting solutions, see:</span></span> 

- [<span data-ttu-id="d3ef6-117">Ei käyttöoikeutta -virheet ja aktivointivirheet Officessa</span><span class="sxs-lookup"><span data-stu-id="d3ef6-117">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [<span data-ttu-id="d3ef6-118">”Emme voi muodostaa yhteyttä tiliisi. Yritä myöhemmin uudelleen" -virhe Officen aktivoinnin yhteydessä</span><span class="sxs-lookup"><span data-stu-id="d3ef6-118">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)