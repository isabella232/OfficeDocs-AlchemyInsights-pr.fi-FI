---
title: Office-tiedoston kaksoisnapsauttaminen ei avaa sitä
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: cd45d64108bc3d7b8f35b51389294f5b8253ba9c
ms.sourcegitcommit: 6df4460313ca033d18b59669506de1dbb7482ef9
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/10/2020
ms.locfileid: "42573521"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="77973-102">Office-tiedoston kaksoisnapsauttaminen ei avaa sitä</span><span class="sxs-lookup"><span data-stu-id="77973-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="77973-103">Kun olet kaksoisnapsauttanut Office-tiedostoa, ohjelma saattaa olla avoinna, mutta itse tiedosto ei avaudu.</span><span class="sxs-lookup"><span data-stu-id="77973-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="77973-104">Tai saatat saada virheilmoituksen: "Komennon lähettämisessä ohjelmaan oli ongelma."</span><span class="sxs-lookup"><span data-stu-id="77973-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="77973-105">Tähän on monia syitä, mutta kaksi yleisintä ratkaisua ovat:</span><span class="sxs-lookup"><span data-stu-id="77973-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="77973-106">Varmista Excelistä, että DDE-asetusta ei ole valittu.</span><span class="sxs-lookup"><span data-stu-id="77973-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="77973-107">Vaihtoehto löytyy luomalla uusi työkirja ja valitsemalla sitten **Tiedosto- > asetukset > Lisäasetukset**.</span><span class="sxs-lookup"><span data-stu-id="77973-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="77973-108">Poista **Yleiset-osassa** **Ohita muut dde (Dynamic Data Exchange) -sovellukset**-valintaruudun valinta.</span><span class="sxs-lookup"><span data-stu-id="77973-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="77973-109">Palauta oletusasetukset suorittamalla online-korjaus.</span><span class="sxs-lookup"><span data-stu-id="77973-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="77973-110">Napsauta Windowsin Käynnistä-painiketta ja etsi hakusanalla "Ohjauspaneeli".</span><span class="sxs-lookup"><span data-stu-id="77973-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="77973-111">Avaa **Ohjauspaneeli**ja siirry **Ohjelmat-> Ohjelmat ja toiminnot -kohtaan**.</span><span class="sxs-lookup"><span data-stu-id="77973-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="77973-112">Napsauta sitten hiiren kakkospainikkeella **Microsoft Office [Versio]** ja valitse **Muuta > Online Repair**.</span><span class="sxs-lookup"><span data-stu-id="77973-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="77973-113">Jos kumpikaan näistä ratkaisuista ei toimi, täydellinen luettelo ratkaisuista on tukiartikkelissa, [Office-tiedoston kaksoisnapsauttaminen ei avaa sitä](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span><span class="sxs-lookup"><span data-stu-id="77973-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
