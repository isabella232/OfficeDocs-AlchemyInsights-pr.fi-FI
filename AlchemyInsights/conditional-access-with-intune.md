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
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36504991"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="e9714-102">Ehdollisen käyttöoikeuden ja Intune</span><span class="sxs-lookup"><span data-stu-id="e9714-102">Conditional Access with Intune</span></span>

<span data-ttu-id="e9714-103">**Ehdollisen käyttöoikeuden** käyttäminen Intune vaatii 3 vaiheet:</span><span class="sxs-lookup"><span data-stu-id="e9714-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="e9714-104">Luo **Ehdollisen käyttöoikeuskäytännön** , joka määrittää, mitä resursseja suojataan, ja ehdot on täytettävä käyttämään kyseisiä resursseja.</span><span class="sxs-lookup"><span data-stu-id="e9714-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="e9714-105">Esimerkiksi laitteen on oltava yhteensopiva ennen yrityksen sähköpostin käyttämistä.</span><span class="sxs-lookup"><span data-stu-id="e9714-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="e9714-106">Voit määrittää asetukset, jotka on täytettävä, ennen kuin laite yhteensopiva katsotaan **Käytännön noudattamista** luominen.</span><span class="sxs-lookup"><span data-stu-id="e9714-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="e9714-107">Esimerkiksi laitteen on oltava vähintään 6 numeroa PIN-koodi ennen kuin se katsotaan yhteensopiva.</span><span class="sxs-lookup"><span data-stu-id="e9714-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="e9714-108">Varmistaminen sekä **Yhteensopivuus** ja **Ehdollinen Access käytännöt** kohdennetut haluamasi käyttäjät ryhmiin.</span><span class="sxs-lookup"><span data-stu-id="e9714-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="e9714-109">Tämä saattaa edellyttää tietyn käyttäjäryhmän luominen Azure Active Directoryssa.</span><span class="sxs-lookup"><span data-stu-id="e9714-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="e9714-110">Lue lisää:</span><span class="sxs-lookup"><span data-stu-id="e9714-110">Read more:</span></span>
  
- [<span data-ttu-id="e9714-111">Ehdollinen Access parhaat käytännöt</span><span class="sxs-lookup"><span data-stu-id="e9714-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="e9714-112">Ehdollisen käytön aloittaminen</span><span class="sxs-lookup"><span data-stu-id="e9714-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

