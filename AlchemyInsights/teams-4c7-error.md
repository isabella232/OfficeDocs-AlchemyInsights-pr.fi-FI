---
title: Teams 4c7-virhe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796088"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="25e5b-102">4c7-virhe Microsoft Teamsissa</span><span class="sxs-lookup"><span data-stu-id="25e5b-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="25e5b-103">Tämä virhe ilmenee, koska Microsoft teams edellyttää lomakkeiden todennusta.</span><span class="sxs-lookup"><span data-stu-id="25e5b-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="25e5b-104">Kun otat käyttöön Active Directory Federation Servicesin (AD FS), lomakkeiden todennus ei oletusarvoisesti ole käytössä intranetissä.</span><span class="sxs-lookup"><span data-stu-id="25e5b-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="25e5b-105">Jos Windowsin integroitu todennus epäonnistuu, sinua kehotetaan Kirjautu maan sisään käyttämällä lomakkeiden todennusta.</span><span class="sxs-lookup"><span data-stu-id="25e5b-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="25e5b-106">Voit ratkaista tämän ongelman ottamalla lomakkeiden todennuksen käyttöön käyttämällä MMC (AD FS Microsoft Management Console)-laajennusta tieto koneessa, jossa on Active Directoryn paikallinen kopio.</span><span class="sxs-lookup"><span data-stu-id="25e5b-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="25e5b-107">Voit tehdä tämän seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="25e5b-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="25e5b-108">Siirry siirtymis ruudussa **todennus käytäntöihin**.</span><span class="sxs-lookup"><span data-stu-id="25e5b-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="25e5b-109">Valitse tiedot-ruudun **toiminnot** -kohdasta **Muokkaa yleistä ensisijaista todennusta**.</span><span class="sxs-lookup"><span data-stu-id="25e5b-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="25e5b-110">Valitse **intranet** -väli lehdestä **lomakkeiden todennus**.</span><span class="sxs-lookup"><span data-stu-id="25e5b-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="25e5b-111">Valitse **OK** (tai **Käytä**).</span><span class="sxs-lookup"><span data-stu-id="25e5b-111">Select **OK** (or **Apply**).</span></span>