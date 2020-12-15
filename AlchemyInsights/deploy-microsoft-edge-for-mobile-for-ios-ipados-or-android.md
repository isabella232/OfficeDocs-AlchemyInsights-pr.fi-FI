---
title: Ota Microsoft Edge for Mobile käyttöön iOS/iPadOS-tai Android-laitteissa
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003919"
- "6974"
ms.openlocfilehash: 98ab637b6ca0f2b3cfa98ae897d6ed1d9f36c3cd
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/11/2020
ms.locfileid: "49678452"
---
# <a name="deploy-microsoft-edge-for-mobile-for-iosipados-or-android"></a><span data-ttu-id="64636-102">Ota Microsoft Edge for Mobile käyttöön iOS/iPadOS-tai Android-laitteissa</span><span class="sxs-lookup"><span data-stu-id="64636-102">Deploy Microsoft Edge for Mobile for iOS/iPadOS or Android</span></span>

<span data-ttu-id="64636-103">Alla olevan ohjatun skenaarion yhteenvedon avulla voit määrittää Microsoft Edgeen iOS:n, iPadOS-ja Android-laitteiden käyttäjille.</span><span class="sxs-lookup"><span data-stu-id="64636-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span> <span data-ttu-id="64636-104">Kun olet suorittanut nämä vaiheet, Microsoft Intune-käytännöt antavat seuraavat Microsoft Edge for Businessin ominaisuudet:</span><span class="sxs-lookup"><span data-stu-id="64636-104">After you complete these steps, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="64636-105">Kaksoiskäyttäjä</span><span class="sxs-lookup"><span data-stu-id="64636-105">Dual identity</span></span>
- <span data-ttu-id="64636-106">Integrointi Microsoft Intune-sovelluksen suojaus käytäntöön</span><span class="sxs-lookup"><span data-stu-id="64636-106">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="64636-107">Integrointi Azure Active Directory-sovelluksen välitys palvelimeen</span><span class="sxs-lookup"><span data-stu-id="64636-107">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="64636-108">Hallitut Suosikit ja aloitus sivun pikanäppäimet</span><span class="sxs-lookup"><span data-stu-id="64636-108">Managed favorites and home page shortcuts</span></span>

> [!NOTE]
> <span data-ttu-id="64636-109">Jos olet torjunut käyttäjiä ilmoittamasta mobiililaitteita, tämä ohjattu toiminto ei toimi, ja käyttäjien on asennettava Microsoft Edge itse.</span><span class="sxs-lookup"><span data-stu-id="64636-109">If you blocked users from enrolling mobile devices, this guided scenario will not work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="64636-110">Jos haluat ottaa Microsoft Edge for Mobilen käyttöön iOS/iPadOS-tai Android-laitteissa, Katso:</span><span class="sxs-lookup"><span data-stu-id="64636-110">To deploy Microsoft Edge for Mobile for iOS/iPadOS or Android, see:</span></span>

1. [<span data-ttu-id="64636-111">Ennakkovaatimukset</span><span class="sxs-lookup"><span data-stu-id="64636-111">Prerequisites</span></span>](https://go.microsoft.com/fwlink/?linkid=2133027)
2. [<span data-ttu-id="64636-112">Johdanto</span><span class="sxs-lookup"><span data-stu-id="64636-112">Introduction</span></span>](https://go.microsoft.com/fwlink/?linkid=2133520)
3. [<span data-ttu-id="64636-113">Perusteet</span><span class="sxs-lookup"><span data-stu-id="64636-113">Basics</span></span>](https://go.microsoft.com/fwlink/?linkid=2133421)
4. [<span data-ttu-id="64636-114">Määritys</span><span class="sxs-lookup"><span data-stu-id="64636-114">Configuration</span></span>](https://go.microsoft.com/fwlink/?linkid=2133521)
5. [<span data-ttu-id="64636-115">Vara ukset</span><span class="sxs-lookup"><span data-stu-id="64636-115">Assignments</span></span>](https://go.microsoft.com/fwlink/?linkid=2132869)
6. [<span data-ttu-id="64636-116">Tarkistaminen ja luominen</span><span class="sxs-lookup"><span data-stu-id="64636-116">Review and creation</span></span>](https://go.microsoft.com/fwlink/?linkid=2133522)
