---
title: Ehdollinen käyttö Intunen kanssa
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706018"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="7dd52-102">Ehdollinen käyttö Intunen kanssa</span><span class="sxs-lookup"><span data-stu-id="7dd52-102">Conditional Access with Intune</span></span>

<span data-ttu-id="7dd52-103">**Ehdollisen käytön** käyttäminen Intunen kanssa vaatii kolme vaihetta:</span><span class="sxs-lookup"><span data-stu-id="7dd52-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="7dd52-104">Luo **ehdollisen käytön käytäntö,** joka määrittää, mitä resursseja suojataan ja mitä ehtoja on täytettävä, jotta resursseja voidaan käyttää.</span><span class="sxs-lookup"><span data-stu-id="7dd52-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="7dd52-105">Laitteen on esimerkiksi oltava yhteensopiva ennen yrityksen sähköpostin käyttöä.</span><span class="sxs-lookup"><span data-stu-id="7dd52-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="7dd52-106">Luo **yhteensopivuuskäytäntö,** joka määrittää asetukset, jotka on täytettävä, ennen kuin laitetta pidetään yhteensopivana.</span><span class="sxs-lookup"><span data-stu-id="7dd52-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="7dd52-107">Laitteen pin-koodin on esimerkiksi oltava vähintään 6 numeroa, ennen kuin sitä pidetään vaatimustenmukaisena.</span><span class="sxs-lookup"><span data-stu-id="7dd52-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="7dd52-108">Yhteensopivuuskäytäntöjen **Compliance Policies** ja **ehdollisen käytön käytäntöjen** kohdistaminen haluttuihin käyttäjäryhmiin.</span><span class="sxs-lookup"><span data-stu-id="7dd52-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="7dd52-109">Tämä saattaa edellyttää tiettyjen käyttäjäryhmien luomista Azure Active Directoryyn.</span><span class="sxs-lookup"><span data-stu-id="7dd52-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="7dd52-110">Lue lisää:</span><span class="sxs-lookup"><span data-stu-id="7dd52-110">Read more:</span></span>
  
- [<span data-ttu-id="7dd52-111">Ehdollisen käytön parhaat käytännöt</span><span class="sxs-lookup"><span data-stu-id="7dd52-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="7dd52-112">Ehdollisen käytön käytön aloittaminen</span><span class="sxs-lookup"><span data-stu-id="7dd52-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

