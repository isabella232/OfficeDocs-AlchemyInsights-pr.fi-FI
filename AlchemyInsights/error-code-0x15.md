---
title: Virhekoodi 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Jos saat virheilmoituksen aktivoidessasi Office 2013:n etätyöpöytäpalveluiden (RDS) käyttöönotoissa, harkitse ADAL-joukkojen käyttöönottoa muokkaamalla rekisteriä.
ms.openlocfilehash: 468d13e59602cf173ed2e17af44c66babfc28703
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506843"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="1a717-103">Virhe aktivoitaessa Office 2013:a etätyöpöytäpalveluissa</span><span class="sxs-lookup"><span data-stu-id="1a717-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="1a717-104">Jos saat virheilmoituksen aktivoidessasi Office 2013:n etätyöpöytäpalveluiden (RDS) käyttöönotoissa, harkitse ADAL-joukkojen käyttöönottoa muokkaamalla rekisteriä.</span><span class="sxs-lookup"><span data-stu-id="1a717-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="1a717-105">**Rekisteriavain**</span><span class="sxs-lookup"><span data-stu-id="1a717-105">**Registry key**</span></span>|<span data-ttu-id="1a717-106">**Tyyppi**</span><span class="sxs-lookup"><span data-stu-id="1a717-106">**Type**</span></span>|<span data-ttu-id="1a717-107">**Arvo**</span><span class="sxs-lookup"><span data-stu-id="1a717-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1a717-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="1a717-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="1a717-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="1a717-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="1a717-110">1</span><span class="sxs-lookup"><span data-stu-id="1a717-110">1</span></span>  <br/> |

<span data-ttu-id="1a717-111">Lisätietoja on ohjeaiheessa [Office 2013:n nykyaikaisen todennuksen ottaminen käyttöön Windows-laitteissa](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="1a717-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="1a717-112">ADAL on oletusarvoisesti käytössä Microsoft 365 Apps for Enterprisessa ja Office 2016:ssa.</span><span class="sxs-lookup"><span data-stu-id="1a717-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="1a717-113">Etätyöpöytäpalvelut (RDS) nimettiin aiemmin päätepalveluille.</span><span class="sxs-lookup"><span data-stu-id="1a717-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  