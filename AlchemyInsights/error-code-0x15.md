---
title: Virhekoodi 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Jos Virhe otettaessa käyttöön Remote Desktop Services (RDS)-Office-2013, harkitse ADAL käyttöön muokkaamalla rekisteriä.
ms.openlocfilehash: 89f9270169e13fd7706f7826c624ef8ae4d47b3f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/15/2019
ms.locfileid: "28286922"
---
<span data-ttu-id="542cf-103">Jos Virhe otettaessa käyttöön Remote Desktop Services (RDS)-Office-2013, harkitse ADAL käyttöön muokkaamalla rekisteriä.</span><span class="sxs-lookup"><span data-stu-id="542cf-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="542cf-104">**Rekisteriavain**</span><span class="sxs-lookup"><span data-stu-id="542cf-104">**Registry key**</span></span>|<span data-ttu-id="542cf-105">**Tyyppi**</span><span class="sxs-lookup"><span data-stu-id="542cf-105">**Type**</span></span>|<span data-ttu-id="542cf-106">**Arvo**</span><span class="sxs-lookup"><span data-stu-id="542cf-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="542cf-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="542cf-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="542cf-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="542cf-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="542cf-109">1</span><span class="sxs-lookup"><span data-stu-id="542cf-109">1</span></span>  <br/> |
   
<span data-ttu-id="542cf-110">Lisätietoja [Office 2013 Windows-laitteiden käyttöön Nykyaikainen todennus](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="542cf-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="542cf-p101">ADAL on käytössä oletusarvoisesti ProPlus Office 365: n ja Office-2016. > Etätyöpöytäpalvelut (RDS) oli ennen nimeltään päätepalvelut.</span><span class="sxs-lookup"><span data-stu-id="542cf-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

