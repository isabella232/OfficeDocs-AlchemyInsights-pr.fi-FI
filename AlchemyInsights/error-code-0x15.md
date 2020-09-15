---
title: Virhe koodi 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: 'Jos saat virhe ilmoituksen, kun Akti voit Office 2013: n Etätyöpöytäpalvelujen (RDS) käyttöönotoissa, harkitse ADALIN ottamista käyttöön muokkaamalla rekisteriä.'
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709184"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="d23b2-103">Virhe Office 2013-sovelluksen Akti voinnin yhteydessä Etätyöpöytäpalveluissa</span><span class="sxs-lookup"><span data-stu-id="d23b2-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="d23b2-104">Jos saat virhe ilmoituksen, kun Akti voit Office 2013: n Etätyöpöytäpalvelujen (RDS) käyttöönotoissa, harkitse ADALIN ottamista käyttöön muokkaamalla rekisteriä.</span><span class="sxs-lookup"><span data-stu-id="d23b2-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="d23b2-105">**Rekisteriavain**</span><span class="sxs-lookup"><span data-stu-id="d23b2-105">**Registry key**</span></span>|<span data-ttu-id="d23b2-106">**Tyyppi**</span><span class="sxs-lookup"><span data-stu-id="d23b2-106">**Type**</span></span>|<span data-ttu-id="d23b2-107">**Arvo**</span><span class="sxs-lookup"><span data-stu-id="d23b2-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d23b2-108">HKEY_CURRENT_USER \Software\microsoft\office\15.0\common\identyt\enableadal</span><span class="sxs-lookup"><span data-stu-id="d23b2-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="d23b2-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="d23b2-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="d23b2-110">1</span><span class="sxs-lookup"><span data-stu-id="d23b2-110">1</span></span>  <br/> |

<span data-ttu-id="d23b2-111">Lisä tietoja on Ohje aiheessa [Office 2013: n modernin todennuksen ottaminen käyttöön Windows-laitteissa](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="d23b2-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="d23b2-112">ADAL on oletusarvoisesti käytössä Microsoft 365-sovelluksissa yritys käyttöön ja Office 2016-sovellukseen.</span><span class="sxs-lookup"><span data-stu-id="d23b2-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="d23b2-113">Etätyöpöytä palvelut (RDS) nimettiin aiemmin pääte palveluina.</span><span class="sxs-lookup"><span data-stu-id="d23b2-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  