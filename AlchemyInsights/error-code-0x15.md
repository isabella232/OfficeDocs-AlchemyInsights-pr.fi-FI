---
title: Virhekoodi 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Jos Virhe otettaessa käyttöön Remote Desktop Services (RDS)-Office-2013, harkitse ADAL käyttöön muokkaamalla rekisteriä.
ms.openlocfilehash: 4ef2943e5a529368fa2c614e4431cf180924fbb8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36526985"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="4a3f4-103">Remote Desktop Services Office 2013 aktivointi virhe</span><span class="sxs-lookup"><span data-stu-id="4a3f4-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="4a3f4-104">Jos Virhe otettaessa käyttöön Remote Desktop Services (RDS)-Office-2013, harkitse ADAL käyttöön muokkaamalla rekisteriä.</span><span class="sxs-lookup"><span data-stu-id="4a3f4-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="4a3f4-105">**Rekisteriavain**</span><span class="sxs-lookup"><span data-stu-id="4a3f4-105">**Registry key**</span></span>|<span data-ttu-id="4a3f4-106">**Tyyppi**</span><span class="sxs-lookup"><span data-stu-id="4a3f4-106">**Type**</span></span>|<span data-ttu-id="4a3f4-107">**Arvo**</span><span class="sxs-lookup"><span data-stu-id="4a3f4-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="4a3f4-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="4a3f4-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="4a3f4-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="4a3f4-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="4a3f4-110">1</span><span class="sxs-lookup"><span data-stu-id="4a3f4-110">1</span></span>  <br/> |

<span data-ttu-id="4a3f4-111">Lisätietoja [Office 2013 Windows-laitteiden käyttöön Nykyaikainen todennus](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="4a3f4-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="4a3f4-112">ADAL on käytössä oletusarvoisesti ProPlus Office 365: n ja Office-2016.</span><span class="sxs-lookup"><span data-stu-id="4a3f4-112">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="4a3f4-113">Remote Desktop Services (RDS) oli ennen nimeltään päätepalvelut.</span><span class="sxs-lookup"><span data-stu-id="4a3f4-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  