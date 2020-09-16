---
title: SharePointin suuret luettelot
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 1bc891a912c6753ea6c85d7d4b2a5d802080bd5c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720130"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="e8ec1-102">Suurten luetteloiden ja kirjastojen käyttäminen SharePointissa</span><span class="sxs-lookup"><span data-stu-id="e8ec1-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="e8ec1-103">SharePoint-luetteloissa ja-kirjastoissa voi olla enintään 30 000 000 kohdetta, mutta kun niillä on yli 5 000 kohdetta, näkyviin voi tulla luettelo näkymän kynnys virhe, kun yrität käsitellä niitä.</span><span class="sxs-lookup"><span data-stu-id="e8ec1-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="e8ec1-104">Tämä raja-arvo on käytössä palvelun suorituskyvyn säilyttämistä varten.</span><span class="sxs-lookup"><span data-stu-id="e8ec1-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="e8ec1-105">Sitä ei voi muuttaa.</span><span class="sxs-lookup"><span data-stu-id="e8ec1-105">It can't be changed.</span></span> <span data-ttu-id="e8ec1-106">Jos et halua lyödä tätä rajaa:</span><span class="sxs-lookup"><span data-stu-id="e8ec1-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="e8ec1-107">**Käytä modernia**</span><span class="sxs-lookup"><span data-stu-id="e8ec1-107">**Use modern**</span></span>

<span data-ttu-id="e8ec1-108">Näkymät, joissa on useita kohteita, toimivat parhaiten modernissa käyttö kokemuksessa.</span><span class="sxs-lookup"><span data-stu-id="e8ec1-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="e8ec1-109">[Käytä modernia käyttö kokemusta](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) , jotta voit välttää virheet, jotka näkyvät perinteisessä käyttö kokemuksessa.</span><span class="sxs-lookup"><span data-stu-id="e8ec1-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="e8ec1-110">**Indeksien lisääminen**</span><span class="sxs-lookup"><span data-stu-id="e8ec1-110">**Add indexes**</span></span>

<span data-ttu-id="e8ec1-111">Kun suodatat tai lajittelet sen sarakkeen mukaan, jossa ei ole indeksiä, näyttöön voi tulla virhe sanoma.</span><span class="sxs-lookup"><span data-stu-id="e8ec1-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="e8ec1-112">[Lisää indeksi](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manuaalisesti asetukset-valikon **luettelo asetuksista** ja sitten **indeksoiduista sarakkeista**.</span><span class="sxs-lookup"><span data-stu-id="e8ec1-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="e8ec1-113">**Luettelon näkymän muokkaaminen**</span><span class="sxs-lookup"><span data-stu-id="e8ec1-113">**Edit the list view**</span></span>

<span data-ttu-id="e8ec1-114">Jos suurella luettelolla on virhe, [Muokkaa luetteloa](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="e8ec1-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="e8ec1-115">Seuraavat neljä muutosta poistavat luettelon näkymän kynnys virheet.</span><span class="sxs-lookup"><span data-stu-id="e8ec1-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="e8ec1-116">Tee kaikki neljä muutosta poistaaksesi kaikki virheet.</span><span class="sxs-lookup"><span data-stu-id="e8ec1-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="e8ec1-117">Jos virheet jatkuvat, tarkista [suurten luetteloiden ja kirjastojen hallinta](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="e8ec1-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="e8ec1-118">Valitse **ei mitään** -vaihto ehdoista **ensin sarakkeen mukaan** ja **Lajittele sitten sarakkeen mukaan**.</span><span class="sxs-lookup"><span data-stu-id="e8ec1-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="e8ec1-119">Valitse **ei mitään** **ensimmäisestä ryhmästä sarakkeen mukaan** ja **Ryhmittele sitten sarakkeen**mukaan.</span><span class="sxs-lookup"><span data-stu-id="e8ec1-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="e8ec1-120">Valitse **ei mitään** kaikkien sarakkeiden **summat** -osiossa.</span><span class="sxs-lookup"><span data-stu-id="e8ec1-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="e8ec1-121">Poista kaikki paitsi yksi sarake näytettäväksi **sarakkeet** -osassa.</span><span class="sxs-lookup"><span data-stu-id="e8ec1-121">Deselect all but one column for display from the **Columns** section.</span></span>

