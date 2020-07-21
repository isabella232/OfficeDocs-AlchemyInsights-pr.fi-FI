---
title: Ristiriidat SourceAnchorin, ProxyAddressin ja UserPrincipalName
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1699"
- "1300022"
ms.openlocfilehash: 826dfe9e5c7d24ff5186a94e1ada4dad536e7edd
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198174"
---
# <a name="conflicts-with-sourceanchor-proxyaddress-userprincipalname"></a><span data-ttu-id="174a2-102">Ristiriidat SourceAnchorin, ProxyAddressin ja UserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="174a2-102">Conflicts with SourceAnchor, ProxyAddress, UserPrincipalName</span></span>

<span data-ttu-id="174a2-103">Jos synkronoinnin aikana ilmenee virheitä, kuten "Synkronoitu objekti, jolla on sama ProxyAddress tai UserPrincipalName, on hakemistossasi," katso [Lisätietoja ohjeaiheesta Kaksoiskappaleiden synkronointivirheiden diagnosointi ja korjaaminen](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span><span class="sxs-lookup"><span data-stu-id="174a2-103">If you receive errors during a synchronization such as "A synchronized object with the same ProxyAddress or UserPrincipalName exists in your directory", see [Diagnose and remediate duplicated attribute sync errors](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span></span>

<span data-ttu-id="174a2-104">Harkitse myös päällekkäisten attribuuttien sietokyvyn käyttöönottoa.</span><span class="sxs-lookup"><span data-stu-id="174a2-104">Also, consider enabling duplicate attribute resiliency.</span></span> <span data-ttu-id="174a2-105">Lisätietoja on kohdassa [Identity synchronization and duplicate attribute resiliency](https://aka.ms/duplicateattributeresiliency).</span><span class="sxs-lookup"><span data-stu-id="174a2-105">For more info, see [Identity synchronization and duplicate attribute resiliency](https://aka.ms/duplicateattributeresiliency).</span></span>