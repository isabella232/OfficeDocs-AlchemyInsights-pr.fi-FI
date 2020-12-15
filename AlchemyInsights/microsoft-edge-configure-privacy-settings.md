---
title: Microsoft Edge tieto suoja-asetusten määrittäminen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677252"
---
# <a name="microsoft-edge-configure-privacy-settings"></a><span data-ttu-id="0aec2-102">Microsoft Edge tieto suoja-asetusten määrittäminen</span><span class="sxs-lookup"><span data-stu-id="0aec2-102">Microsoft Edge configure privacy settings</span></span>

<span data-ttu-id="0aec2-103">Oletusarvoisesti jos Microsoft Edge on käytössä muissa kuin Windows-ympäristöissä, diagnostiikka tietoja ja sivuston tietoja ei lähetetä Microsoftille.</span><span class="sxs-lookup"><span data-stu-id="0aec2-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information are not sent to Microsoft.</span></span> <span data-ttu-id="0aec2-104">Jos Microsoft Edge on otettu käyttöön Windows 10: ssä, diagnostiikka tiedot ja sivuston tiedot lähetetään käyttäjän [Windows Diagnostic Data-asetusten](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)mukaisesti.</span><span class="sxs-lookup"><span data-stu-id="0aec2-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span></span>

<span data-ttu-id="0aec2-105">Jos haluat määrittää, miten Microsoft Edge käsittelee organisaation tietojen keräämistä, käytä seuraavia ryhmä käytäntöjä:</span><span class="sxs-lookup"><span data-stu-id="0aec2-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="0aec2-106">[Metromicsportagenabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): Tämä käytäntö mahdollistaa käytön ja kaatumis tietoihin liittyvien tietojen ilmoittamisen.</span><span class="sxs-lookup"><span data-stu-id="0aec2-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): This policy enables reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="0aec2-107">[Sendsiteinfotoimproveservices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): Tämä toiminto lähettää sivuston tietoja, joita käytetään Microsoftin palveluiden parantamiseen.</span><span class="sxs-lookup"><span data-stu-id="0aec2-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): This policy sends site information that is used to improve Microsoft services.</span></span>

<span data-ttu-id="0aec2-108">Lisä tietoja on Ohje aiheessa [käytäntöjen asetusten määrittäminen](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span><span class="sxs-lookup"><span data-stu-id="0aec2-108">To learn more, see [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span></span>