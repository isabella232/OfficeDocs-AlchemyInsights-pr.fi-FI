---
title: 1490-vian määritys-eDiscoveryn virheet
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277814"
---
# <a name="troubleshoot-content-search-errors"></a><span data-ttu-id="b5bc1-102">Sisältö haun virheiden vian määritys</span><span class="sxs-lookup"><span data-stu-id="b5bc1-102">Troubleshoot Content Search errors</span></span>

<span data-ttu-id="b5bc1-103">Onko sinulla ongelmia sisältö haussa tai virheiden saamisessa haku tuloksia vietäessä?</span><span class="sxs-lookup"><span data-stu-id="b5bc1-103">Are you experiencing problems with Content Search or getting failures when you export search results?</span></span>

<span data-ttu-id="b5bc1-104">Oletko esimerkiksi saanut seuraavat haut, kun suoritat hakuja?</span><span class="sxs-lookup"><span data-stu-id="b5bc1-104">For example, are you receiving the following when running searches?</span></span>

- <span data-ttu-id="b5bc1-105">CS008-tai CS012-virheet</span><span class="sxs-lookup"><span data-stu-id="b5bc1-105">CS008 or CS012 errors</span></span>

- <span data-ttu-id="b5bc1-106">Palvelin varattu/aika katkaisu virheet</span><span class="sxs-lookup"><span data-stu-id="b5bc1-106">Server busy/timeout errors</span></span>

- <span data-ttu-id="b5bc1-107">Sovellus virhe ilmeni</span><span class="sxs-lookup"><span data-stu-id="b5bc1-107">Application error occurred</span></span>

<span data-ttu-id="b5bc1-108">Tai haettaessa tai vietäessä tuloksia suuresta määrästä posti laatikoita (yli 100 000 posti laatikkoa), Saatko vienti virheitä?</span><span class="sxs-lookup"><span data-stu-id="b5bc1-108">Or when searching or exporting results from a large number of mailboxes (over 100,000 mailboxes), are you getting export errors?</span></span>

<span data-ttu-id="b5bc1-109">Jos kyseessä on virhe, yritä etsiä uudelleen epäonnistuneita sisältö sijainteja.</span><span class="sxs-lookup"><span data-stu-id="b5bc1-109">For these types of errors, retry the search for the content locations that have failed.</span></span> <span data-ttu-id="b5bc1-110">Katso lisä tietoja  [tästä artikkelista](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="b5bc1-110">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>

<span data-ttu-id="b5bc1-111">Jos viet yli 100 000 posti laatikkoa, sinun on ladattava vienti tulokset seuraavan PowerShellin avulla: vie  [tulokset yli 100k posti laatikosta](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="b5bc1-111">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>
