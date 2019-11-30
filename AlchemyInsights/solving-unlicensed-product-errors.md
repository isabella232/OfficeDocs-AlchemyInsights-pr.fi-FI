---
title: Ei-lisensoitujen tuote virheiden ratkaiseminen
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
ms.openlocfilehash: 178811c81775b22676a0106283be4e516d40a95b
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628023"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a><span data-ttu-id="e3496-102">Ehdotuksia "Lisensoitumattomia tuotteita" koskevien virheiden ratkaisemiseksi</span><span class="sxs-lookup"><span data-stu-id="e3496-102">Suggestions for solving "Unlicensed Product" errors</span></span>

<span data-ttu-id="e3496-103">Voit ratkaista "Lisensoitumattomia tuotteita" koskevia virheitä seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="e3496-103">To solve errors about an "Unlicensed Product," try the following:</span></span>

- <span data-ttu-id="e3496-104">Tarkista, onko tilauksesi tila vanhentunut.</span><span class="sxs-lookup"><span data-stu-id="e3496-104">Check to see if your subscription status has expired.</span></span>
- <span data-ttu-id="e3496-105">Varmista, että sinulla on tilaus, joka sallii asiakkaan käyttö oikeudet, kuten Office 365 Business tai Business Premium, ja varmista, [että käyttäjälle on määritetty käyttö oikeus](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="e3496-105">Make sure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure that the user has a license assigned](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users).</span></span> 
- <span data-ttu-id="e3496-106">Varmista, että käyttäjä on kirjautunut sisään Officeen samalla tilillä, jolle on määritetty käyttö oikeus.</span><span class="sxs-lookup"><span data-stu-id="e3496-106">Make sure the user is signing in to Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="e3496-107">Tarkista [Office 365 Service Health-sivulta](https://docs.microsoft.com/office365/enterprise/view-service-health) , onko palvelussa tunnettuja ongelmia.</span><span class="sxs-lookup"><span data-stu-id="e3496-107">Check the [Office 365 Service health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="e3496-108">Tarkista palo muuri-, virustentorjuntaohjelmisto-ja välitys palvelin asetukset ja varmista, etteivät ne estä Office-sovellusten pääsyä Internetiin.</span><span class="sxs-lookup"><span data-stu-id="e3496-108">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Office apps access to the Internet.</span></span> <span data-ttu-id="e3496-109">Katso [Office 365-URL-osoitteet ja IP-osoite alueet](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="e3496-109">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

<span data-ttu-id="e3496-110">Voit myös kokeilla seuraavia vian määritys toimia:</span><span class="sxs-lookup"><span data-stu-id="e3496-110">You may also try the following troubleshooting actions:</span></span> 

- <span data-ttu-id="e3496-111">Avaa Office-sovellus ja [Kirjaudu ulos](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) aiemmin luodusta käyttäjä tileistä.</span><span class="sxs-lookup"><span data-stu-id="e3496-111">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="e3496-112">[Poista](https://docs.microsoft.com/office365/admin/manage/remove-licenses-from-users) Office [-](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) käyttö oikeus ja määritä se uudelleen ja kirjaudu sitten sisään [Officeen](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) käyttämällä kyseistä käyttäjä tiliä.</span><span class="sxs-lookup"><span data-stu-id="e3496-112">[Remove](https://docs.microsoft.com/office365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) the Office license, and then [sign in to Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="e3496-113">Suorita [Akti voinnin vian määritys](https://aka.ms/SARA-OfficeActivation-Alchemy).</span><span class="sxs-lookup"><span data-stu-id="e3496-113">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy).</span></span>
- <span data-ttu-id="e3496-114">[Palauta Officen aktivointi tila](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="e3496-114">[Reset the Office activation state](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span> 
- <span data-ttu-id="e3496-115">[Suorita Officen online-korjaus](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span><span class="sxs-lookup"><span data-stu-id="e3496-115">[Perform an Online Repair of Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span></span>

<span data-ttu-id="e3496-116">Lisä vian määritys ratkaisuja on kohdassa:</span><span class="sxs-lookup"><span data-stu-id="e3496-116">For additional troubleshooting solutions, see:</span></span> 

- [<span data-ttu-id="e3496-117">Lisensoitu tuote-ja aktivointi virheet Officessa</span><span class="sxs-lookup"><span data-stu-id="e3496-117">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [<span data-ttu-id="e3496-118">"Pahoittelemme, emme voi muodostaa yhteyttä tiliisi. Yritä myöhemmin uudelleen "-virhe, kun Akti voit Officen</span><span class="sxs-lookup"><span data-stu-id="e3496-118">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)