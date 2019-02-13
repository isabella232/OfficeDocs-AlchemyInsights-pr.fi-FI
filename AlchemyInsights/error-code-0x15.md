---
title: Virhekoodi 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Jos Virhe otettaessa käyttöön Remote Desktop Services (RDS)-Office-2013, harkitse ADAL käyttöön muokkaamalla rekisteriä.
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/12/2019
ms.locfileid: "29929085"
---
<span data-ttu-id="6e3a8-103">Jos Virhe otettaessa käyttöön Remote Desktop Services (RDS)-Office-2013, harkitse ADAL käyttöön muokkaamalla rekisteriä.</span><span class="sxs-lookup"><span data-stu-id="6e3a8-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="6e3a8-104">**Rekisteriavain**</span><span class="sxs-lookup"><span data-stu-id="6e3a8-104">**Registry key**</span></span>|<span data-ttu-id="6e3a8-105">**Tyyppi**</span><span class="sxs-lookup"><span data-stu-id="6e3a8-105">**Type**</span></span>|<span data-ttu-id="6e3a8-106">**Arvo**</span><span class="sxs-lookup"><span data-stu-id="6e3a8-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="6e3a8-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="6e3a8-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="6e3a8-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="6e3a8-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="6e3a8-109">1</span><span class="sxs-lookup"><span data-stu-id="6e3a8-109">1</span></span>  <br/> |
   
<span data-ttu-id="6e3a8-110">Lisätietoja [Office 2013 Windows-laitteiden käyttöön Nykyaikainen todennus](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="6e3a8-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="6e3a8-p101">ADAL on käytössä oletusarvoisesti ProPlus Office 365: n ja Office-2016. remote Desktop Services (RDS) > oli ennen nimeltään päätepalvelut.</span><span class="sxs-lookup"><span data-stu-id="6e3a8-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

