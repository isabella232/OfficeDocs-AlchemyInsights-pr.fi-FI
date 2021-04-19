---
title: Vanhojen valintaikkunoiden upottamisen ottaminen käyttöön raporttien avaamista varten
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814261"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="bb832-102">Vanhojen valintaikkunoiden upottamisen ottaminen käyttöön raporttien avaamista varten</span><span class="sxs-lookup"><span data-stu-id="bb832-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="bb832-103">**Oire**</span><span class="sxs-lookup"><span data-stu-id="bb832-103">**Symptom**</span></span>

<span data-ttu-id="bb832-104">Käyttäjät eivät voi avata raportteja.</span><span class="sxs-lookup"><span data-stu-id="bb832-104">Users are unable to open reports.</span></span> <span data-ttu-id="bb832-105">"Jokin on mennyt vikaan.</span><span class="sxs-lookup"><span data-stu-id="bb832-105">"Something has gone wrong.</span></span> <span data-ttu-id="bb832-106">Katso lisätietoja teknisistä kohdista."</span><span class="sxs-lookup"><span data-stu-id="bb832-106">Check technical details for more details."</span></span>

<span data-ttu-id="bb832-107">**Syy**</span><span class="sxs-lookup"><span data-stu-id="bb832-107">**Cause**</span></span>

<span data-ttu-id="bb832-108">Raportit eivät lataudu NÄYTTÖÖN ja virheilmoitus "Lomakkeen kuvaaja on tyhjäarvo tai sitä ei ole määritetty".</span><span class="sxs-lookup"><span data-stu-id="bb832-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="bb832-109">FU:n raportit edellyttävät edelleen vanhoja valintaikkuntoja, joten asiakkaan järjestelmässä on oltava *allowlegacydialogsedding käytössä.*</span><span class="sxs-lookup"><span data-stu-id="bb832-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="bb832-110">**Ratkaisu**</span><span class="sxs-lookup"><span data-stu-id="bb832-110">**Solution**</span></span>

1. <span data-ttu-id="bb832-111">Valitse Asetukset **>hallinta > Järjestelmäasetukset-> Yleiset-välilehti.**</span><span class="sxs-lookup"><span data-stu-id="bb832-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="bb832-112">Määritä "Ota tiettyjen vanhojen valintaikkunoiden upottaminen käyttöön yhdistetyn käyttöliittymän selainasiakasohjelmassa" -arvoksi **Kyllä.**</span><span class="sxs-lookup"><span data-stu-id="bb832-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
