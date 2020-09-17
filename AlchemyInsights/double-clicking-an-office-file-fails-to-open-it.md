---
title: Office-tiedoston kaksoisnapsauttaminen ei avaa sitä
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
- "2200002"
- "161"
ms.openlocfilehash: 9dc4196cd36c8682e4d047e8abad493be97ced3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812076"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="fb259-102">Office-tiedoston kaksoisnapsauttaminen ei avaa sitä</span><span class="sxs-lookup"><span data-stu-id="fb259-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="fb259-103">Kun olet kaksoisnapsauttanut Office-tiedostoa, saatat nähdä ohjelman avautuvan, mutta tiedosto ei avaudu.</span><span class="sxs-lookup"><span data-stu-id="fb259-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="fb259-104">Näyttöön voi tulla virhe sanoma, jossa on ilmennyt ongelma ohjelman lähetyksessä.</span><span class="sxs-lookup"><span data-stu-id="fb259-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="fb259-105">Tähän on monia syitä, mutta kaksi yleisintä ratkaisua ovat seuraavat:</span><span class="sxs-lookup"><span data-stu-id="fb259-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="fb259-106">Varmista Excel-ohjelmassa, että DDE-vaihto ehto ei ole valittuna.</span><span class="sxs-lookup"><span data-stu-id="fb259-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="fb259-107">Vaihto ehto löytyy luomalla uusi työkirja ja valitsemalla sitten **tiedosto > asetukset > Advanced**.</span><span class="sxs-lookup"><span data-stu-id="fb259-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="fb259-108">Poista **Yleiset** -osiossa valinta kohdasta **Älä huomioi muita sovelluksia, jotka käyttävät dynaamista tietojen vaihtamista (DDE)**.</span><span class="sxs-lookup"><span data-stu-id="fb259-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="fb259-109">Palauta oletus asetukset suorittamalla online-korjaus.</span><span class="sxs-lookup"><span data-stu-id="fb259-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="fb259-110">Napsauta Windowsin Käynnistä-painiketta ja Etsi "ohjaus paneeli".</span><span class="sxs-lookup"><span data-stu-id="fb259-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="fb259-111">Avaa **ohjaus paneeli**ja valitse **ohjelmat > ohjelmat ja toiminnot**.</span><span class="sxs-lookup"><span data-stu-id="fb259-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="fb259-112">Napsauta sitten hiiren kakkos painikkeella kohtaa **Microsoft Office [versio]** ja valitse **Muuta > online-korjaus**.</span><span class="sxs-lookup"><span data-stu-id="fb259-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="fb259-113">Jos kumpikaan näistä ratkaisuista ei toimi, täydellinen ratkaisu luettelo löytyy tuki-artikkelista, jolloin [Office-tiedostoa ei voi avata kaksoisnapsauttamalla sitä](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span><span class="sxs-lookup"><span data-stu-id="fb259-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
