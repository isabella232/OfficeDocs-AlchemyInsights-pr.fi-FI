---
title: Active Directory ei synkronoidu
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
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822848"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="d4c05-102">Active Directory ei synkronoidu</span><span class="sxs-lookup"><span data-stu-id="d4c05-102">Active Directory not syncing</span></span>

<span data-ttu-id="d4c05-103">Jos saat synkronointivirheitä, kuten "ei viimeaikaista synkronointia", tai huomaat Hakemistosynkronoinnin tilan Office-hallintaportaalissa, jossa lukee "Viimeksi synkronoitu yli kolme päivää sitten", AADConnectissa voi olla virheellisiä asetuksia tai liian vähän käyttöoikeuksia synkronoinnin suorittamiseen.</span><span class="sxs-lookup"><span data-stu-id="d4c05-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="d4c05-104">AADConnectin uudelleenasentaminen pika-asetusten avulla voi ratkaista ongelman nopeasti:</span><span class="sxs-lookup"><span data-stu-id="d4c05-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="d4c05-105">[Lataa uusin AADConnect-versio.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="d4c05-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="d4c05-106">[Noudata pika-asennuksen ohjeita.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="d4c05-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="d4c05-107">Lisätietoja AADConnect -palvelutileistä on kohdassa [Azure AD Connect: Tilit ja käyttöoikeudet.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)</span><span class="sxs-lookup"><span data-stu-id="d4c05-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
