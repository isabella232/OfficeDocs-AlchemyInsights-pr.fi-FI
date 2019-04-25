---
title: Ehdollisen käyttöoikeuden ja Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32393538"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="e2d07-102">Ehdollisen käyttöoikeuden ja Intune</span><span class="sxs-lookup"><span data-stu-id="e2d07-102">Conditional Access with Intune</span></span>

<span data-ttu-id="e2d07-103">**Ehdollisen käyttöoikeuden** käyttäminen Intune vaatii 3 vaiheet:</span><span class="sxs-lookup"><span data-stu-id="e2d07-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="e2d07-104">Luo **Ehdollisen käyttöoikeuskäytännön** , joka määrittää, mitä resursseja suojataan, ja ehdot on täytettävä käyttämään kyseisiä resursseja.</span><span class="sxs-lookup"><span data-stu-id="e2d07-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="e2d07-105">Esimerkiksi laitteen on oltava yhteensopiva ennen yrityksen sähköpostin käyttämistä.</span><span class="sxs-lookup"><span data-stu-id="e2d07-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="e2d07-106">Voit määrittää asetukset, jotka on täytettävä, ennen kuin laite yhteensopiva katsotaan **Käytännön noudattamista** luominen.</span><span class="sxs-lookup"><span data-stu-id="e2d07-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="e2d07-107">Esimerkiksi laitteen on oltava vähintään 6 numeroa PIN-koodi ennen kuin se katsotaan yhteensopiva.</span><span class="sxs-lookup"><span data-stu-id="e2d07-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="e2d07-108">Varmistaminen sekä **Yhteensopivuus** ja **Ehdollinen Access käytännöt** kohdennetut haluamasi käyttäjät ryhmiin.</span><span class="sxs-lookup"><span data-stu-id="e2d07-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="e2d07-109">Tämä saattaa edellyttää tietyn käyttäjäryhmän luominen Azure Active Directoryssa.</span><span class="sxs-lookup"><span data-stu-id="e2d07-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="e2d07-110">Lue lisää:</span><span class="sxs-lookup"><span data-stu-id="e2d07-110">Read more:</span></span>
  
- [<span data-ttu-id="e2d07-111">Ehdollinen Access parhaat käytännöt</span><span class="sxs-lookup"><span data-stu-id="e2d07-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="e2d07-112">Ehdollisen käytön aloittaminen</span><span class="sxs-lookup"><span data-stu-id="e2d07-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

