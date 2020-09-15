---
title: Teamsin 4c7-virhe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700200"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="f40d6-102">4c7-virhe Microsoft Teamsissa</span><span class="sxs-lookup"><span data-stu-id="f40d6-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="f40d6-103">Tämä virhe johtuu siitä, että Microsoft teams edellyttää lomakkeiden todennusta.</span><span class="sxs-lookup"><span data-stu-id="f40d6-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="f40d6-104">Kun otat käyttöön Active Directory-liittoutumis palveluja (AD FS), lomakkeiden todennus ei ole oletusarvoisesti käytössä intranetiin.</span><span class="sxs-lookup"><span data-stu-id="f40d6-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="f40d6-105">Jos Windowsin integroitu todennus epäonnistuu, sinua pyydetään Kirjautu maan sisään käyttämällä lomakkeiden todennusta.</span><span class="sxs-lookup"><span data-stu-id="f40d6-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="f40d6-106">Ratkaise ongelma ottamalla käyttöön lomakkeiden todentaminen käyttämällä Microsoft Management Console (MMC)-laajennusta tieto koneessa, jossa on paikallinen kopio Active Directorysta.</span><span class="sxs-lookup"><span data-stu-id="f40d6-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="f40d6-107">Voit tehdä tämän seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="f40d6-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="f40d6-108">Etsi siirtymis ruudussa **todennus käytännöt**.</span><span class="sxs-lookup"><span data-stu-id="f40d6-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="f40d6-109">Valitse tieto ruudun **toiminnot** -kohdassa **Muokkaa yleistä päätodennusta**.</span><span class="sxs-lookup"><span data-stu-id="f40d6-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="f40d6-110">Valitse **intranet** -väli lehdessä **lomakkeiden todennus**.</span><span class="sxs-lookup"><span data-stu-id="f40d6-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="f40d6-111">Valitse **OK** (tai **Käytä**).</span><span class="sxs-lookup"><span data-stu-id="f40d6-111">Select **OK** (or **Apply**).</span></span>