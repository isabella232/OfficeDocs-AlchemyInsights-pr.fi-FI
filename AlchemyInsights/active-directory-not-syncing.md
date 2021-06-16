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
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930972"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="b9fd4-102">Active Directory ei synkronoidu</span><span class="sxs-lookup"><span data-stu-id="b9fd4-102">Active Directory not syncing</span></span>

<span data-ttu-id="b9fd4-103">Jos saat synkronointivirheitä, kuten "ei viimeaikaista synkronointia", tai huomaat hakemistosynkronoinnin tilan Office-hallintaportaalissa, jossa lukee "Viimeksi synkronoitu yli kolme päivää sitten", AADConnectissa voi olla virheellisiä asetuksia tai liian vähän käyttöoikeuksia synkronoinnin suorittamiseen.</span><span class="sxs-lookup"><span data-stu-id="b9fd4-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="b9fd4-104">AADConnectin uudelleenasentaminen pika-asetusten avulla voi ratkaista ongelman nopeasti:</span><span class="sxs-lookup"><span data-stu-id="b9fd4-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="b9fd4-105">[Lataa uusin AADConnect-versio.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="b9fd4-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="b9fd4-106">[Noudata pika-asennuksen ohjeita.](/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="b9fd4-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="b9fd4-107">Azure AD Connect täytyy asentaa Windows Server 2012:een tai tätä uudempaan.</span><span class="sxs-lookup"><span data-stu-id="b9fd4-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="b9fd4-108">Tämän palvelimen täytyy olla liitetty toimialueeseen. Se voi olla toimialueen ohjauskone tai jäsenpalvelin.</span><span class="sxs-lookup"><span data-stu-id="b9fd4-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="b9fd4-109">Täydellinen luettelo Azure AD-Näyttöyhteys ja edellytyksistä on kohdassa Azure AD Näyttöyhteys: n [edellytykset.](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)</span><span class="sxs-lookup"><span data-stu-id="b9fd4-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="b9fd4-110">Lisätietoja AADConnect -palvelutileistä on kohdassa [Azure AD Näyttöyhteys: Tilit ja käyttöoikeudet.](/azure/active-directory/hybrid/reference-connect-accounts-permissions)</span><span class="sxs-lookup"><span data-stu-id="b9fd4-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
