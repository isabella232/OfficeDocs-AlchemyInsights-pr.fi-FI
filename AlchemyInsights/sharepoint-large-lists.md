---
title: SharePointin suuret luettelot
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 2/12/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 222ad554de0d94dcfd4e34e9a2c6aa8ab4e6f81f
ms.sourcegitcommit: d7e1b097d3866782f508527c797426dc56c6ba17
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/14/2019
ms.locfileid: "37488514"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="26805-102">Suurten luetteloiden ja kirjastojen työskentely SharePointissa</span><span class="sxs-lookup"><span data-stu-id="26805-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="26805-103">SharePoint-luettelot ja-kirjastot voivat sisältää enintään 30 000 000 kohdetta, mutta kun niissä on yli 5 000 kohdetta, luettelo näkymän kynnys virhe voi olla, kun yrität käsitellä niitä.</span><span class="sxs-lookup"><span data-stu-id="26805-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="26805-104">Tämä kynnys on käytössä palvelun suoritus kyvyn ylläpitämiseksi.</span><span class="sxs-lookup"><span data-stu-id="26805-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="26805-105">Sitä ei voi muuttaa.</span><span class="sxs-lookup"><span data-stu-id="26805-105">It can't be changed.</span></span> <span data-ttu-id="26805-106">Välttääksesi tämän kynnyksen lyömisen:</span><span class="sxs-lookup"><span data-stu-id="26805-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="26805-107">**Käytä modernia**</span><span class="sxs-lookup"><span data-stu-id="26805-107">**Use modern**</span></span>

<span data-ttu-id="26805-108">Monet kohteet näyttävät parhaiten modernissa kokemuksella.</span><span class="sxs-lookup"><span data-stu-id="26805-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="26805-109">[Käytä modernia kokemusta](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) välttääksesi virheitä, joita saatat nähdä klassisessa kokemuksessa.</span><span class="sxs-lookup"><span data-stu-id="26805-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="26805-110">**Indeksien lisääminen**</span><span class="sxs-lookup"><span data-stu-id="26805-110">**Add indexes**</span></span>

<span data-ttu-id="26805-111">Kun suodatat tai lajittelet sellaisen sarakkeen mukaan, jolla ei ole indeksiä, saatat nähdä virhe sanoman.</span><span class="sxs-lookup"><span data-stu-id="26805-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="26805-112">[Lisää indeksi](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manuaalisesti asetukset-valikon **luettelo asetuksista** ja sitten **Indeksoidut sarakkeet**.</span><span class="sxs-lookup"><span data-stu-id="26805-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="26805-113">**Muokkaa luettelo näkymää**</span><span class="sxs-lookup"><span data-stu-id="26805-113">**Edit the list view**</span></span>

<span data-ttu-id="26805-114">Jos suurta luetteloa käsiteltäessä tapahtuu virhe, [Muokkaa luettelo näkymää](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="26805-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="26805-115">Seuraavat neljä muutosta poistavat luettelo näkymän kynnys virheet.</span><span class="sxs-lookup"><span data-stu-id="26805-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="26805-116">Poista kaikki virheet tekemällä kaikki neljä muutosta.</span><span class="sxs-lookup"><span data-stu-id="26805-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="26805-117">Jos virheitä on yhä, tarkista [suurten luetteloiden ja kirjastojen hallinta](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="26805-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="26805-118">Valitse **ei mitään** **sarakkeen ensimmäisestä lajittelussa** ja **Lajittele sitten sarakkeen mukaan**.</span><span class="sxs-lookup"><span data-stu-id="26805-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="26805-119">Valitse **sarakkeen ensimmäisestä ryhmästä** **ei mitään** ja **Ryhmittele sitten sarakkeen mukaan**.</span><span class="sxs-lookup"><span data-stu-id="26805-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="26805-120">Valitse kaikki **summat** -osan sarakkeissa **ei mitään** .</span><span class="sxs-lookup"><span data-stu-id="26805-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="26805-121">Poista valinta kohdasta Kaikki paitsi yksi sarake näytääksesi **sarakkeet** -osasta.</span><span class="sxs-lookup"><span data-stu-id="26805-121">Deselect all but one column for display from the **Columns** section.</span></span>

