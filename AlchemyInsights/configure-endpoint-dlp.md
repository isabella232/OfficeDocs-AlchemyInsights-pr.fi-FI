---
title: Päätepisteen DLP-asetuksen määrittäminen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 039c8f78c5896b66eab5763fb0bbddd3f0b06f2d
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/03/2020
ms.locfileid: "46555128"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="f5f03-102">Päätepisteen DLP-asetuksen määrittäminen</span><span class="sxs-lookup"><span data-stu-id="f5f03-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="f5f03-103">Microsoft Endpoint DLP:n avulla voit laajentaa DLP-suojaus- ja valvontaominaisuuksia arkaluonteisiin tietoihin Windows 10 -laitteissa.</span><span class="sxs-lookup"><span data-stu-id="f5f03-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="f5f03-104">Kun laitteet on otettu laitteen hallintaan, voit luoda DLP-käytäntöjä kohteiden suojaamistoimien valvomiseksi.</span><span class="sxs-lookup"><span data-stu-id="f5f03-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="f5f03-105">Activity Explorerin avulla voidaan valvoa arkaluonteisten kohteiden toimintaa.</span><span class="sxs-lookup"><span data-stu-id="f5f03-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="f5f03-106">Lisätietoja on [ohjeaiheessa Laitteiden onminen laitteiden hallintaan](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="f5f03-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="f5f03-107">Päätepisteen DLP-käytön aloittaminen:</span><span class="sxs-lookup"><span data-stu-id="f5f03-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="f5f03-108">Varmista, että sinulla on asianmukainen SKU/subscriptions-käyttöoikeus.</span><span class="sxs-lookup"><span data-stu-id="f5f03-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="f5f03-109">Lisätietoja on kohdassa [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="f5f03-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="f5f03-110">Tarkista laitteen hallinnan käyttöönottoon tarvittavat käyttöoikeudet, siirry perehdytyssivulle tai ota laitteen valvonta käyttöön tai poista se käytöstä.</span><span class="sxs-lookup"><span data-stu-id="f5f03-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="f5f03-111">Lisätietoja on kohdassa [Käyttöoikeudet](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="f5f03-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="f5f03-112">Laitteiden osaksi Laitteen hallinta noudattamalla perehdytyslaitteiden menettely.</span><span class="sxs-lookup"><span data-stu-id="f5f03-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="f5f03-113">Jos et näe M365-yhteensopivuusasetusten Laitenautelu (esikatselu) -vaihtoehtoa, varmista, että sinulla on edellä mainitut käyttöoikeudet. **Settings**</span><span class="sxs-lookup"><span data-stu-id="f5f03-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="f5f03-114">Lisätietoja on kohdassa [Perehdytyslaitteet](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="f5f03-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="f5f03-115">Luo DLP-käytäntöjä, jotka suojaavat arkaluonteisia kohteita.</span><span class="sxs-lookup"><span data-stu-id="f5f03-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="f5f03-116">Lisätietoja on kohdassa [Päätepisteen DLP-käytäntöskenaariot](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="f5f03-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="f5f03-117">Lisätietoja Microsoft Endpoint DLP:stä on ohjeaiheessa [Lisätietoja Microsoft 365 Endpoint -tietojen menetyksen estämisestä (esikatselu)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="f5f03-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>