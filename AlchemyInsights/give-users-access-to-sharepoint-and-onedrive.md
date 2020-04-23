---
title: SharePointin ja OneDriven käyttöoikeuksien salliminen käyttäjille
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 0bdc2fa97ad1fe8b3280411babaaf2bd685a644d
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43721742"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="61775-102">SharePointin ja OneDriven käyttöoikeuksien salliminen käyttäjille</span><span class="sxs-lookup"><span data-stu-id="61775-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="61775-103">Jos OneDrive- tai SharePoint-sivusto ei ole useiden käyttäjien käytettävissä aiemmin, palveluongelma saattaa olla tilapäinen.</span><span class="sxs-lookup"><span data-stu-id="61775-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="61775-104">Tarkista palvelun kunnon koontinäyttö</span><span class="sxs-lookup"><span data-stu-id="61775-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="61775-105">Jos haluat, että organisaatiosi käyttäjät voivat kirjautua sisään ja käyttää SharePointia ja OneDrivea, sinun on lisättävä heille tilejä ja varmistettava, että heillä on käyttöoikeus, joka antaa heille oikeuden käyttää SharePointia ja OneDrivea.</span><span class="sxs-lookup"><span data-stu-id="61775-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="61775-106">Helpoin tapa lisätä käyttäjiä on Microsoft 365 -hallintakeskuksessa.</span><span class="sxs-lookup"><span data-stu-id="61775-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="61775-107">Siirry [Microsoft 365 -hallintakeskuksen Aktiiviset käyttäjät -sivulle](https://portal.office.com/adminportal/home#/users)ja valitse sitten **Lisää käyttäjä**.</span><span class="sxs-lookup"><span data-stu-id="61775-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="61775-108">Täytä käyttäjän tiedot ja varmista, että **Tuotteen käyttöoikeudet**-kohdassa määritetään käyttöoikeus ja **SharePoint Online** on valittuna.</span><span class="sxs-lookup"><span data-stu-id="61775-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="61775-109">Huomaa, että jos sallit ulkoisen jakamisen organisaatiossasi, käyttäjät voivat jakaa SharePoint- ja OneDrive-sisältöä organisaation ulkopuolisten henkilöiden kanssa.</span><span class="sxs-lookup"><span data-stu-id="61775-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="61775-110">Sinun ei tarvitse antaa näille ulkoisille käyttäjille käyttöoikeuksia.</span><span class="sxs-lookup"><span data-stu-id="61775-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="61775-111">Sinun ei myöskään tarvitse lisätä tilejä niille, ellei jakaminen ole "Vain olemassa olevat ulkoiset käyttäjät".</span><span class="sxs-lookup"><span data-stu-id="61775-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="61775-112">Jos ihmiset eivät ole organisaatiosi hakemistossa, sinun on lisättävä heidät vieraskäyttäjiksi Azure AD -hallintakeskukseen.</span><span class="sxs-lookup"><span data-stu-id="61775-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

