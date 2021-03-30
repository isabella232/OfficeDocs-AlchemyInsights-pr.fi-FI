---
title: Tietosuoja-asetusten määrittäminen Microsoft Edgessä
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404617"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a><span data-ttu-id="b25e9-102">Tietosuoja-asetusten määrittäminen Microsoft Edgessä</span><span class="sxs-lookup"><span data-stu-id="b25e9-102">Configure privacy settings in Microsoft Edge</span></span>

<span data-ttu-id="b25e9-103">Jos Microsoft Edge otetaan käyttöön ei-Windows-käyttöympäristöissä, diagnostiikkatietoja ja sivuston tietoja ei oletusarvoisesti lähetetä Microsoftille.</span><span class="sxs-lookup"><span data-stu-id="b25e9-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information aren't sent to Microsoft.</span></span> <span data-ttu-id="b25e9-104">Jos Microsoft Edge otetaan käyttöön Windows 10:ssä, diagnostiikkatiedot ja sivustotiedot lähetetään käyttäjien [Windowsin diagnostiikkatietojen asetusten mukaan.](https://go.microsoft.com/fwlink/?linkid=2132472)</span><span class="sxs-lookup"><span data-stu-id="b25e9-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://go.microsoft.com/fwlink/?linkid=2132472).</span></span>

<span data-ttu-id="b25e9-105">Jos haluat määrittää, miten Microsoft Edge käsittelee organisaatiosi tietojen keräämistä, käytä seuraavia ryhmäkäytäntöjä:</span><span class="sxs-lookup"><span data-stu-id="b25e9-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="b25e9-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) ottaa käyttöön käytön ja kaatumiseen liittyvien tietojen raportoinnin.</span><span class="sxs-lookup"><span data-stu-id="b25e9-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) turns on reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="b25e9-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) lähettää sivuston tietoja, joita käytetään Microsoft-palvelujen parantamiseen.</span><span class="sxs-lookup"><span data-stu-id="b25e9-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sends site information used to improve Microsoft services.</span></span>

<span data-ttu-id="b25e9-108">Lisätietoja on kohdassa [Käytäntöasetusten määrittäminen.](https://go.microsoft.com/fwlink/?linkid=2132577)</span><span class="sxs-lookup"><span data-stu-id="b25e9-108">To learn more, see [Configure policy settings](https://go.microsoft.com/fwlink/?linkid=2132577).</span></span>
