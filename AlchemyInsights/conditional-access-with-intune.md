---
title: Ehdollisen käyttöoikeuden ja Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 3b50bc96a879017b62e42e1849f72e68408a0d9d
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/30/2019
ms.locfileid: "29662324"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="ecc8f-102">Ehdollisen käyttöoikeuden ja Intune</span><span class="sxs-lookup"><span data-stu-id="ecc8f-102">Conditional Access with Intune</span></span>

<span data-ttu-id="ecc8f-103">**Ehdollisen käyttöoikeuden** käyttäminen Intune vaatii 3 vaiheet:</span><span class="sxs-lookup"><span data-stu-id="ecc8f-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="ecc8f-p101">Luo **Ehdollisen käyttöoikeuskäytännön** , joka määrittää, mitä resursseja suojataan, ja ehdot on täytettävä käyttämään kyseisiä resursseja. Esimerkiksi laitteen on oltava yhteensopiva ennen yrityksen sähköpostin käyttämistä.</span><span class="sxs-lookup"><span data-stu-id="ecc8f-p101">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="ecc8f-p102">Voit määrittää asetukset, jotka on täytettävä, ennen kuin laite yhteensopiva katsotaan **Käytännön noudattamista** luominen. Esimerkiksi laitteen on oltava vähintään 6 numeroa PIN-koodi ennen kuin se katsotaan yhteensopiva.</span><span class="sxs-lookup"><span data-stu-id="ecc8f-p102">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="ecc8f-p103">Varmistaminen sekä **Yhteensopivuus** ja **Ehdollinen Access käytännöt** kohdennetut haluamasi käyttäjät ryhmiin. Tämä saattaa edellyttää tietyn käyttäjäryhmän luominen Azure Active Directoryssa.</span><span class="sxs-lookup"><span data-stu-id="ecc8f-p103">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="ecc8f-110">Lue lisää:</span><span class="sxs-lookup"><span data-stu-id="ecc8f-110">Read more:</span></span>
  
- [<span data-ttu-id="ecc8f-111">Ehdollinen Access parhaat käytännöt</span><span class="sxs-lookup"><span data-stu-id="ecc8f-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="ecc8f-112">Ehdollisen käytön aloittaminen</span><span class="sxs-lookup"><span data-stu-id="ecc8f-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

