---
title: SharePointin ja OneDriven käyttö oikeuksien antaminen käyttäjille
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a7e9c0b7ffa5c11a2e24ee5fda6491f049f985f1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677204"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="2a5b4-102">SharePointin ja OneDriven käyttö oikeuksien antaminen käyttäjille</span><span class="sxs-lookup"><span data-stu-id="2a5b4-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="2a5b4-103">Jos OneDrive-tai SharePoint-sivusto ei ole käytettävissä useille käyttäjille, joilla on aiemmin ollut käyttö oikeus, kyseessä saattaa olla väliaikainen palvelu ongelma.</span><span class="sxs-lookup"><span data-stu-id="2a5b4-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="2a5b4-104">Palvelun kunnon koonti näytön tarkistaminen</span><span class="sxs-lookup"><span data-stu-id="2a5b4-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="2a5b4-105">Jos haluat, että organisaation käyttäjät voivat kirja utua sisään ja käyttää SharePointia ja OneDrivea, sinun on lisättävä heidän tilejään ja varmistettava, että heillä on käyttö oikeus, jonka avulla he voivat käyttää SharePointia ja OneDrivea.</span><span class="sxs-lookup"><span data-stu-id="2a5b4-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="2a5b4-106">Helpoin tapa lisätä käyttäjiä on Microsoft 365-hallinta keskuksessa.</span><span class="sxs-lookup"><span data-stu-id="2a5b4-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="2a5b4-107">Siirry [Microsoft 365-hallinta keskuksen aktiiviset käyttäjät-sivulle](https://portal.office.com/adminportal/home#/users)ja valitse sitten **Lisää käyttäjä**.</span><span class="sxs-lookup"><span data-stu-id="2a5b4-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="2a5b4-108">Täytä käyttäjän tiedot ja varmista, että **tuotteen käyttö oikeudet**-kohdassa on määritetty käyttö oikeus ja että **SharePoint Online** on valittuna.</span><span class="sxs-lookup"><span data-stu-id="2a5b4-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="2a5b4-109">Huomaa, että jos sallit ulkoista jakamista organisaatiossasi, käyttäjät voivat jakaa SharePointin ja OneDriven sisältöä organisaation ulkopuolisten henkilöiden kanssa.</span><span class="sxs-lookup"><span data-stu-id="2a5b4-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="2a5b4-110">Sinun ei tarvitse antaa näille ulkoisille käyttäjille käyttö oikeuksia.</span><span class="sxs-lookup"><span data-stu-id="2a5b4-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="2a5b4-111">Sinun ei myöskään tarvitse lisätä tilejäsi, ellei jakamis asetukseksi ole valittu vain olemassa olevia ulkoisia käyttäjiä.</span><span class="sxs-lookup"><span data-stu-id="2a5b4-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="2a5b4-112">Siinä tapa uksessa, jos henkilöt eivät ole organisaatiosi hakemistossa, sinun on lisättävä heidät vieras käyttäjiksi Azure AD-hallinta keskuksessa.</span><span class="sxs-lookup"><span data-stu-id="2a5b4-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

