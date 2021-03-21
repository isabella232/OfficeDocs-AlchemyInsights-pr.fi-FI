---
title: Microsoft Defenderin päätepisteiden koneiden käyttöönotto-ongelmat
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901564"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="c1ba1-102">Microsoft Defenderin päätepisteiden koneiden käyttöönotto-ongelmat</span><span class="sxs-lookup"><span data-stu-id="c1ba1-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="c1ba1-103">Sinulla voi olla ongelmia koneiden MDE-palvelun käyttöönotossa.</span><span class="sxs-lookup"><span data-stu-id="c1ba1-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="c1ba1-104">Jos pääset loppukäyttäjän tietokoneelle, toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="c1ba1-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="c1ba1-105">Lataa uusin[MDE Client Analyzer](https://aka.ms/betamdeanalyzer) -diagnostiikkatyökalun esiversio.</span><span class="sxs-lookup"><span data-stu-id="c1ba1-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="c1ba1-106">Napsauta **MDEClientAnalyzer.cmd** hiiren kakkospainikkeella ja valitse Suorita järjestelmänvalvojana.</span><span class="sxs-lookup"><span data-stu-id="c1ba1-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="c1ba1-107">Noudata **MDEClientAnalyzer.htm** -sivulla annettuja ohjeita.</span><span class="sxs-lookup"><span data-stu-id="c1ba1-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="c1ba1-108">Jos haluat yksityiskohtaisempia lokeja, tutustu **MDEClientAnalyzerResult** nimiseen alikansioon.</span><span class="sxs-lookup"><span data-stu-id="c1ba1-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="c1ba1-109">Jos tarvitset lisäohjeita, ota yhteyttä [Microsoft Defender for Endpointin tukipalveluun](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) ja anna tuloksena saatava MDEClientAnalyzerResult.zip-tiedosto analyysia varten.</span><span class="sxs-lookup"><span data-stu-id="c1ba1-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
