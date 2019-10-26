---
title: Ehdollinen pääsy Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/25/2019
ms.locfileid: "36504991"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="282c0-102">Ehdollinen pääsy Intune</span><span class="sxs-lookup"><span data-stu-id="282c0-102">Conditional Access with Intune</span></span>

<span data-ttu-id="282c0-103">**Ehdollisen käytön** käyttäminen Intune-toiminnolla edellyttää 3 vaihetta:</span><span class="sxs-lookup"><span data-stu-id="282c0-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="282c0-104">Luo **Ehdollinen käyttö oikeus käytäntö** , joka määrittää, mitä resursseja suojataan ja mitkä ehdot on täytettävä näiden resurssien käyttöä varten.</span><span class="sxs-lookup"><span data-stu-id="282c0-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="282c0-105">Laitteen on esimerkiksi oltava yhteensopiva ennen yrityksen sähkö postin käyttämistä.</span><span class="sxs-lookup"><span data-stu-id="282c0-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="282c0-106">Luo yhteensopivuus käytäntö määrittääksesi asetukset, joiden on täytyttävä, ennen kuin laite katsotaan **yhteensopivaksi** .</span><span class="sxs-lookup"><span data-stu-id="282c0-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="282c0-107">Laitteessa on esimerkiksi oltava vähintään 6-merkkinen PIN-tunnus, ennen kuin se katsotaan yhteensopivaksi.</span><span class="sxs-lookup"><span data-stu-id="282c0-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="282c0-108">Sekä **yhteensopivuus käytäntöjen** että **ehdollisten käyttö oikeus käytäntöjen** varmistaminen on suunnattu halutulle käyttäjä ryhmille.</span><span class="sxs-lookup"><span data-stu-id="282c0-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="282c0-109">Tämä saattaa edellyttää tiettyjen käyttäjä ryhmien luomista Azure Active Directoryyn.</span><span class="sxs-lookup"><span data-stu-id="282c0-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="282c0-110">Lue lisää:</span><span class="sxs-lookup"><span data-stu-id="282c0-110">Read more:</span></span>
  
- [<span data-ttu-id="282c0-111">Ehdollisen käytön parhaat käytännöt</span><span class="sxs-lookup"><span data-stu-id="282c0-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="282c0-112">Ehdollisen käytön aloittaminen</span><span class="sxs-lookup"><span data-stu-id="282c0-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

