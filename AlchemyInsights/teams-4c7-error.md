---
title: Teams 4c7 -virhe
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
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786666"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="cce1d-102">4c7-virhe Microsoft Teamsissa</span><span class="sxs-lookup"><span data-stu-id="cce1d-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="cce1d-103">Tämä virhe ilmenee, koska Microsoft Teams edellyttää Forms-todennusta.</span><span class="sxs-lookup"><span data-stu-id="cce1d-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="cce1d-104">Kun otat Active Directory Federation Servicesin (AD FS) käyttöön, lomakkeiden todennus ei ole oletusarvoisesti käytössä intranetissä.</span><span class="sxs-lookup"><span data-stu-id="cce1d-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="cce1d-105">Jos Windows Integrated Authentication epäonnistuu, sinua pyydetään kirjautumaan sisään käyttämällä Forms-todennusta.</span><span class="sxs-lookup"><span data-stu-id="cce1d-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="cce1d-106">Voit ratkaista tämän ongelman käyttäen AD FS Microsoft Management Console (MMC) -laajennusta tietokoneessa, jossa on paikallinen Active Directory -versio, käyttäen lomakkeiden todennusta.</span><span class="sxs-lookup"><span data-stu-id="cce1d-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="cce1d-107">Voit tehdä tämän seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="cce1d-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="cce1d-108">Valitse siirtymisruudussa **Todennuskäytännöt.**</span><span class="sxs-lookup"><span data-stu-id="cce1d-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="cce1d-109">Valitse **tietoruudun** Toiminnot-kohdassa Muokkaa **yleisessä ensisijaisessa todentamisessa**.</span><span class="sxs-lookup"><span data-stu-id="cce1d-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="cce1d-110">Valitse **Intranet-välilehdessä** **Lomakkeiden todennus**.</span><span class="sxs-lookup"><span data-stu-id="cce1d-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="cce1d-111">Valitse **OK** (tai **Käytä).**</span><span class="sxs-lookup"><span data-stu-id="cce1d-111">Select **OK** (or **Apply**).</span></span>