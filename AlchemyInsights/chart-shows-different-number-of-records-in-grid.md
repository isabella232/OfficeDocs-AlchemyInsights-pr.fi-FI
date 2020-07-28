---
title: Kaaviossa näkyy ruudukon tietueiden eri määrä
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 3d0be28c783bb129d05484565c6c2a56ac5e0acf
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439356"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a><span data-ttu-id="25488-102">Kaaviossa näkyy ruudukon tietueiden eri määrä</span><span class="sxs-lookup"><span data-stu-id="25488-102">Chart shows different number of records in grid</span></span>

<span data-ttu-id="25488-103">**Oire**</span><span class="sxs-lookup"><span data-stu-id="25488-103">**Symptom**</span></span>

<span data-ttu-id="25488-104">Kaavion dashboard-sivulla, kun klikkaat kaaviota "..." ja klikkaa "Näytä tietueet", siirryt ruudukkosivulle nähdäksesi kaikki tietueet. Joskus tietueiden määrä muuttuu.</span><span class="sxs-lookup"><span data-stu-id="25488-104">For chart on dashboard page, when you click on chart "…" and click "View records", you navigate to grid page to see all the records.Sometimes, the number of records changes.</span></span>

<span data-ttu-id="25488-105">**Syy**</span><span class="sxs-lookup"><span data-stu-id="25488-105">**Cause**</span></span>

<span data-ttu-id="25488-106">Tämä johtuu alkuperäisen koontinäytön sivun kaavion ja ruudukon kotisivun kaavion välisten näkymien eroista.</span><span class="sxs-lookup"><span data-stu-id="25488-106">This is due to the difference of views between the chart on the original dashboard page and the chart on the grid home page.</span></span>  

<span data-ttu-id="25488-107">**Ratkaisu**</span><span class="sxs-lookup"><span data-stu-id="25488-107">**Solution**</span></span>

1. <span data-ttu-id="25488-108">Tarkista näkymä alkuperäiseltä sivulta ja ruudukon näkymästä, ovatko ne erilaisia.</span><span class="sxs-lookup"><span data-stu-id="25488-108">Check the view from the original page and the view in the grid to see if they are different.</span></span>
2. <span data-ttu-id="25488-109">Muuta ruudukon näkymä vastaamaan alkuperäisen sivun näkymää.</span><span class="sxs-lookup"><span data-stu-id="25488-109">Change the view in grid to match the view in the original page.</span></span>
3. <span data-ttu-id="25488-110">Jos oikeaa näkymää ei löydy, näkymää ei yleensä ole otettu käyttöön sovelluksen suunnitteluohjelmassa.</span><span class="sxs-lookup"><span data-stu-id="25488-110">If the correct view cannot be found, usually it means the view is not enabled in app designer.</span></span>
4. <span data-ttu-id="25488-111">Siirry tietyn sovelluksen sovelluksen suunnittelijaan, valitse entiteetti ja sen näkymät, tarkista näkymä, jonka haluat ottaa käyttöön, tallentaa, julkaista ja sulkea.</span><span class="sxs-lookup"><span data-stu-id="25488-111">Go to app designer of the specific app, choose the entity and its views, check the view you want to enable, save, publish and close.</span></span>
5. <span data-ttu-id="25488-112">Päivitä sivu.</span><span class="sxs-lookup"><span data-stu-id="25488-112">Refresh the page.</span></span>