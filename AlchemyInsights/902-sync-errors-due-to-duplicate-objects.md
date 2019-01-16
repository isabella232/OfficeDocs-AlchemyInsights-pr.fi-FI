---
title: 902 (synkronointivirheet objektien kaksoisarvot vuoksi)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: f8db233167a5e2b2ef7290438b8e6d92d0dccb1e
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/15/2019
ms.locfileid: "28287258"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="7c42f-102">Samanlaiset objektit synkronointivirheiden</span><span class="sxs-lookup"><span data-stu-id="7c42f-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="7c42f-103">Näyttöön tulee jokin seuraavista virhesanomista, kun directory-synkronointi on valmis:</span><span class="sxs-lookup"><span data-stu-id="7c42f-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>
  
- <span data-ttu-id="7c42f-104">Ei voi päivittää tätä objektia Microsoft Online Services-palveluissa, koska tämän objektin liittyvät seuraavat määritteet ovat arvoja, jotka on ehkä jo liitetty toinen paikallinen hakemisto-objekti.</span><span class="sxs-lookup"><span data-stu-id="7c42f-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>
    
- <span data-ttu-id="7c42f-105">Microsoft Online Services-kansiossa on jo synkronoitu objekti saman välityspalvelimen osoite.</span><span class="sxs-lookup"><span data-stu-id="7c42f-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>
    
- <span data-ttu-id="7c42f-106">Objektia ei voi päivittää tätä, koska tämä objekti liittyy seuraavat määritteet ovat arvoja, jotka voi olla jo liitetty toiseen objektiin paikallisen-hakemistopalveluihin: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="7c42f-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>
    
<span data-ttu-id="7c42f-107">Voit tunnistaa ja korjata ongelman, lataa ja suorita [IdFix DirSync virheen korjaus työkalu](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="7c42f-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>
  
<span data-ttu-id="7c42f-108">Lisätietoja on kohdassa [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="7c42f-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
  

