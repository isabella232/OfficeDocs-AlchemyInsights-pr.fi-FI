---
title: Luo organisaatiosuhde, jonka avulla käyttäjäsi voivat tehdä yhteistyötä toisen organisaation kanssa
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: b595fb87e18a055a7df1ff4c782a93591dd1f024
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816125"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="60171-102">Luo organisaatiosuhde, jonka avulla käyttäjäsi voivat tehdä yhteistyötä toisen organisaation kanssa</span><span class="sxs-lookup"><span data-stu-id="60171-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="60171-103">Siirry Microsoft 365 -hallintakeskuksessa kohtaan **Järjestelmänvalvoja** > **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="60171-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="60171-104">Valitse **Organisaatio** > **Jakaminen**.</span><span class="sxs-lookup"><span data-stu-id="60171-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="60171-105">Valitse **Organisaation jakaminen** -kohdassa **Uusi**</span><span class="sxs-lookup"><span data-stu-id="60171-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="60171-106">Kirjoita **Uusi organisaatiosuhde** -kohdan **Suhteen nimi** -ruutuun organisaatiosuhteen kutsumanimi.</span><span class="sxs-lookup"><span data-stu-id="60171-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="60171-107">Kirjoita **Toimialueet, joiden kanssa jaetaan** -ruutuun sen ulkoisen Office 365- tai paikallisen Exchange-organisaation toimialue, jonka kanssa haluat jakaa kalenterisi.</span><span class="sxs-lookup"><span data-stu-id="60171-107">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars.</span></span> <span data-ttu-id="60171-108">Jos haluat kirjoittaa useamman kuin yhden toimialueen, erota toimialuenimet toisistaan pilkulla.</span><span class="sxs-lookup"><span data-stu-id="60171-108">If you need to enter more than one domain, separate the domain names with a comma.</span></span> <span data-ttu-id="60171-109">Kirjoita esimerkiksi contoso.com, service.contoso.com.</span><span class="sxs-lookup"><span data-stu-id="60171-109">For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="60171-110">Valitse **Ota kalenterin tavoitettavuustietojen jakaminen käyttöön** -valintaruutu, jotta voit jakaa kalenterit luettelemillesi toimialueille.</span><span class="sxs-lookup"><span data-stu-id="60171-110">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed.</span></span> <span data-ttu-id="60171-111">Määritä tavoitettavuustietojen jakamistaso ja se, mitkä käyttäjät voivat jakaa kalenterin tavoitettavuustietoja.</span><span class="sxs-lookup"><span data-stu-id="60171-111">Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="60171-112">Voit määrittää tavoitettavuustietojen jakamistason valitsemalla jonkin seuraavista:</span><span class="sxs-lookup"><span data-stu-id="60171-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="60171-113">**Kalenterin tavoitettavuustiedot ja vain aika**</span><span class="sxs-lookup"><span data-stu-id="60171-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="60171-114">**Kalenterin tavoitettavuustiedot ja aika, aihe sekä sijainti**</span><span class="sxs-lookup"><span data-stu-id="60171-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="60171-115">Voit määrittää, mitkä käyttäjät voivat jakaa kalenterin tavoitettavuustietoja, valitsemalla jonkin seuraavista:</span><span class="sxs-lookup"><span data-stu-id="60171-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="60171-116">**Kaikki organisaation käyttäjät**</span><span class="sxs-lookup"><span data-stu-id="60171-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="60171-117">**Tietty käyttöoikeusryhmä**</span><span class="sxs-lookup"><span data-stu-id="60171-117">**A specified security group**</span></span>  

<span data-ttu-id="60171-118">Valitse **Selaa**, etsi käyttöoikeusryhmä luettelosta ja valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="60171-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="60171-119">Luo organisaatiosuhde valitsemalla **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="60171-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="60171-120">**Huomautus:** Vuokraajien väliset määritykset eivät tue henkilökohtaisia yhteystietoja tavoitettavuustietojen hakemisessa.</span><span class="sxs-lookup"><span data-stu-id="60171-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="60171-121">Yhteystietojen tulee sisältyä yleiseen osoiteluetteloon, jotta tavoitettavuustiedot voidaan hakea.</span><span class="sxs-lookup"><span data-stu-id="60171-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="60171-122">**Katso lisätietoja tästä aiheesta seuraavista artikkeleista:**</span><span class="sxs-lookup"><span data-stu-id="60171-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="60171-123">Organisaatiosuhteen luominen Exchange Onlinessa</span><span class="sxs-lookup"><span data-stu-id="60171-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="60171-124">Organisaatiosuhteen muokkaaminen Exchange Onlinessa</span><span class="sxs-lookup"><span data-stu-id="60171-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="60171-125">Organisaatiosuhteen poistaminen Exchange Onlinessa</span><span class="sxs-lookup"><span data-stu-id="60171-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
