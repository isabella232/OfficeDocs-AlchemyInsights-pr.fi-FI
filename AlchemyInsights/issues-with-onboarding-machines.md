---
title: Perehdytyskoneisiin liittyvät ongelmat
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141466"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="08797-102">Perehdytyskoneisiin liittyvät ongelmat</span><span class="sxs-lookup"><span data-stu-id="08797-102">Issues with onboarding machines</span></span>

<span data-ttu-id="08797-103">MDATP-palveluun liittyvissä koneiden käytössä saattaa olla ongelmia.</span><span class="sxs-lookup"><span data-stu-id="08797-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="08797-104">Jos voit käyttää loppukäyttäjäkonetta, toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="08797-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="08797-105">Lataa [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) -diagnostiikkatyökalu.</span><span class="sxs-lookup"><span data-stu-id="08797-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="08797-106">Pura ja suorita MDATPAnalyzer.cmd.</span><span class="sxs-lookup"><span data-stu-id="08797-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="08797-107">Etsi diagnostiikkaloki kansiosta nimeltä MDATPClientAnalyzerResult, samasta kansiosta, johon Analyzer-työkalu ladataan.</span><span class="sxs-lookup"><span data-stu-id="08797-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="08797-108">Tarkista lokitiedostosta MDATPClientAnalyzer.txt yhteys- tai internet-välityspalvelimen asetukset.</span><span class="sxs-lookup"><span data-stu-id="08797-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>