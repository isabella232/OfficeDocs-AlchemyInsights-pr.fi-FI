---
title: SharePointin suuret luettelot
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: e85686788c60d365a00970e9ffe58e97512894a3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767282"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="2cc05-102">Suurten luetteloiden ja kirjastojen luominen SharePointissa</span><span class="sxs-lookup"><span data-stu-id="2cc05-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="2cc05-103">SharePoint-luetteloissa ja -kirjastoissa voi olla enintään 30 miljoonaa kohdetta, mutta kun niissä on yli 5 000 kohdetta, saatat nähdä luettelonäkymän kynnysarvovirheen, kun yrität käsitellä niitä.</span><span class="sxs-lookup"><span data-stu-id="2cc05-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="2cc05-104">Tämä raja-arvo on käytössä palvelun suorituskyvyn säilyttämistä varten.</span><span class="sxs-lookup"><span data-stu-id="2cc05-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="2cc05-105">Sitä ei voi muuttaa.</span><span class="sxs-lookup"><span data-stu-id="2cc05-105">It can't be changed.</span></span> <span data-ttu-id="2cc05-106">Voit välttää tämän kynnyksen saavuttamisen:</span><span class="sxs-lookup"><span data-stu-id="2cc05-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="2cc05-107">**Käytä nykyaikaisia**</span><span class="sxs-lookup"><span data-stu-id="2cc05-107">**Use modern**</span></span>

<span data-ttu-id="2cc05-108">Näkymät, joissa näkyy monia kohteita, toimivat parhaiten modernissa kokemuksessa.</span><span class="sxs-lookup"><span data-stu-id="2cc05-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="2cc05-109">[Käytä modernia kokemusta](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) välttääksesi virheitä, joita saatat nähdä perinteisessä kokemuksessa.</span><span class="sxs-lookup"><span data-stu-id="2cc05-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="2cc05-110">**Indeksien lisääminen**</span><span class="sxs-lookup"><span data-stu-id="2cc05-110">**Add indexes**</span></span>

<span data-ttu-id="2cc05-111">Kun suodatat tai lajittelet sarakkeen mukaan, jossa ei ole indeksiä, näyttöön saattaa tulee virhesanoma.</span><span class="sxs-lookup"><span data-stu-id="2cc05-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="2cc05-112">[Lisää indeksi](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manuaalisesti asetusvalikon **Luetteloasetukset-kohdasta** ja sitten **Indeksoituja sarakkeita**.</span><span class="sxs-lookup"><span data-stu-id="2cc05-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="2cc05-113">**Luettelonäkymän muokkaaminen**</span><span class="sxs-lookup"><span data-stu-id="2cc05-113">**Edit the list view**</span></span>

<span data-ttu-id="2cc05-114">Jos suuri luettelo -käytössä ilmenee virhe, [muokkaa luettelonäkymää](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="2cc05-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="2cc05-115">Seuraavat neljä muutosta poistavat luettelonäkymän kynnysvirheet.</span><span class="sxs-lookup"><span data-stu-id="2cc05-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="2cc05-116">Poista kaikki virheet kaikista neljästä muutosta.</span><span class="sxs-lookup"><span data-stu-id="2cc05-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="2cc05-117">Jos saat edelleen virheitä, valitse [Suurten luetteloiden ja kirjastojen hallinta](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="2cc05-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="2cc05-118">Valitse **ei mitään** sekä Lajittele ensin sarakkeen **mukaan** että Lajittele sitten **sarakkeen mukaan**.</span><span class="sxs-lookup"><span data-stu-id="2cc05-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="2cc05-119">Valitse **ei mitään** sekä **ensimmäisestä ryhmästä sarakkeen mukaan** että **Ryhmittele sitten sarakkeen mukaan**.</span><span class="sxs-lookup"><span data-stu-id="2cc05-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="2cc05-120">Valitse **Ei mitään** kaikille **Summille-osan** sarakkeille.</span><span class="sxs-lookup"><span data-stu-id="2cc05-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="2cc05-121">Poista kaikkien paitsi yhden sarakkeen valinta **Sarakkeet-osiosta** näytettäväksi.</span><span class="sxs-lookup"><span data-stu-id="2cc05-121">Deselect all but one column for display from the **Columns** section.</span></span>

