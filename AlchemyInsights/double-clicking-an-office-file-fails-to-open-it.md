---
title: Office-tiedoston kaksoisnapsauttaminen ei avaa sitä
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: b9c563f7dd099bf3bad9018f69e2096816dd7290
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814802"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="7187a-102">Office-tiedoston kaksoisnapsauttaminen ei avaa sitä</span><span class="sxs-lookup"><span data-stu-id="7187a-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="7187a-103">Kun olet kaksoisnapsauttanut Office-tiedostoa, saatat nähdä ohjelman avoimena, mutta itse tiedosto ei avaudu.</span><span class="sxs-lookup"><span data-stu-id="7187a-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="7187a-104">Tai saatat saada virhesanoman: "Ilmeni ongelma komennon lähettämisessä ohjelmaan".</span><span class="sxs-lookup"><span data-stu-id="7187a-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="7187a-105">Tähän on monia syitä, mutta kaksi yleisintä ratkaisua ovat seuraavat:</span><span class="sxs-lookup"><span data-stu-id="7187a-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="7187a-106">Varmista Excelissä, että DDE-asetusta ei ole valittu.</span><span class="sxs-lookup"><span data-stu-id="7187a-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="7187a-107">Voit valita vaihtoehdon luomalla uuden työkirjan ja valitsemalla sitten Tiedosto **ja > asetukset > lisäasetukset.**</span><span class="sxs-lookup"><span data-stu-id="7187a-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="7187a-108">Poista **Yleiset-kohdassa** Ohita muut Dynamic **Data Exchange (DDE) -sovelluksia käyttävät sovellukset -valintaruudun valinta.**</span><span class="sxs-lookup"><span data-stu-id="7187a-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="7187a-109">Palauta oletusasetukset suoritamalla Online-korjaus.</span><span class="sxs-lookup"><span data-stu-id="7187a-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="7187a-110">Napsauta Windowsin Käynnistä-painiketta ja tee haku hakusanalla "Ohjauspaneeli".</span><span class="sxs-lookup"><span data-stu-id="7187a-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="7187a-111">Avaa Ohjauspaneeli **ja valitse** Ohjelmat ja > ohjelmat **ja toiminnot**.</span><span class="sxs-lookup"><span data-stu-id="7187a-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="7187a-112">Napsauta sitten hiiren kakkospainikkeella **Microsoft Office [Versio]** ja **valitse Muuta > Online-korjaus .**</span><span class="sxs-lookup"><span data-stu-id="7187a-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="7187a-113">Jos kumpikaan näistä ratkaisuista ei toimi, täydellinen ratkaisuluettelo löytyy tukiartikkelista, [Office-tiedoston](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)kaksoisnapsauttaminen ei avaa sitä.</span><span class="sxs-lookup"><span data-stu-id="7187a-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
