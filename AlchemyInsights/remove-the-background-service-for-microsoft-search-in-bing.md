---
title: Microsoft Searchin taustapalvelun poistaminen Bingissä
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816198"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="63eea-102">Microsoft Searchin taustapalvelun poistaminen Bingissä</span><span class="sxs-lookup"><span data-stu-id="63eea-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="63eea-103">Voit poistaa Microsoft Searchin taustapalvelun Bingissä kokeilemalla seuraavia korjaustoimenpiteitä:</span><span class="sxs-lookup"><span data-stu-id="63eea-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="63eea-104">Voit palauttaa alkuperäiset hakukoneasetukset seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="63eea-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="63eea-105">a.</span><span class="sxs-lookup"><span data-stu-id="63eea-105">a.</span></span> <span data-ttu-id="63eea-106">Vaihda Käytä **Bingiä oletushakukoneena [-vaihtopainike pois](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) käytöstä.**</span><span class="sxs-lookup"><span data-stu-id="63eea-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="63eea-107">b.</span><span class="sxs-lookup"><span data-stu-id="63eea-107">b.</span></span> <span data-ttu-id="63eea-108">[Siirry Microsoft 365 -hallintakeskukseen](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) ja poista asetus, joka vaikuttaa organisaatiosi kaikkiin käyttäjiin.</span><span class="sxs-lookup"><span data-stu-id="63eea-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="63eea-109">Voit poistaa taustapalvelun yksittäisestä laitteesta seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="63eea-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="63eea-110">a.</span><span class="sxs-lookup"><span data-stu-id="63eea-110">a.</span></span> <span data-ttu-id="63eea-111">Valitse **Ohjauspaneeli > ohjelmat > ja toiminnot -kohdassa.**</span><span class="sxs-lookup"><span data-stu-id="63eea-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="63eea-112">b.</span><span class="sxs-lookup"><span data-stu-id="63eea-112">b.</span></span> <span data-ttu-id="63eea-113">Napsauta **Bingissä hiiren kakkospainikkeella Microsoft Searchia** asennettujen ohjelmien luettelossa ja valitse sitten **Poista asennus.**</span><span class="sxs-lookup"><span data-stu-id="63eea-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="63eea-114">Jos haluat poistaa taustapalvelun useista organisaation laitteista, kirjaudu sisään järjestelmänvalvojana ja suorita seuraava komento komentosarjassa:</span><span class="sxs-lookup"><span data-stu-id="63eea-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
