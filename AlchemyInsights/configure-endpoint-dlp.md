---
title: Määritä päätepisteen DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402417"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="3bf73-102">Määritä päätepisteen DLP</span><span class="sxs-lookup"><span data-stu-id="3bf73-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="3bf73-103">Microsoftin päätepisteen DLP sallii sinun laajentaa tietojen menetyksen estämisen suojausta ja arkaluonteisten tietojen valvontakykyä Windows 10 -laitteissa.</span><span class="sxs-lookup"><span data-stu-id="3bf73-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="3bf73-104">Kun laitteet on otettu käyttöön laitteiden hallinnassa, voit luoda DLP-käytäntöjä kohteiden suojaustoimiin.</span><span class="sxs-lookup"><span data-stu-id="3bf73-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="3bf73-105">Toiminnan hallinnassa voit valvoa arkaluonteisten kohteiden toimintaa.</span><span class="sxs-lookup"><span data-stu-id="3bf73-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="3bf73-106">Lisätietoja on kohdassa [Laitteiden käyttöönotto laitteiden hallinnassa](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="3bf73-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="3bf73-107">Jos haluat aloittaa päätepisteen DLP:n käytön:</span><span class="sxs-lookup"><span data-stu-id="3bf73-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="3bf73-108">Varmista, että sinulla on tarvittavat SKU- tai tilauskäyttöoikeudet.</span><span class="sxs-lookup"><span data-stu-id="3bf73-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="3bf73-109">Lisätietoja on kohdassa [SKU- tai tilauskäyttöoikeudet](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="3bf73-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="3bf73-110">Tarkista käyttöoikeudet, jotka vaaditaan laitteiden hallintaan, laitteiden lisäyssivulle pääsyyn tai laitteiden valvonnan käyttöönottoon tai sen käytöstä poistamiseen.</span><span class="sxs-lookup"><span data-stu-id="3bf73-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="3bf73-111">Lisätietoja on kohdassa [Käyttöoikeudet](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="3bf73-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="3bf73-112">Lisää laitteita laitteiden hallintaan noudattamalla laitteiden käyttöönoton toimintosarjaa.</span><span class="sxs-lookup"><span data-stu-id="3bf73-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="3bf73-113">Jos laitteiden käyttöönotto (esikatselu) puuttuu M365:n **yhteensopivuusasetuksista**, varmista, että sinulla on edellä mainitut käyttöoikeudet.</span><span class="sxs-lookup"><span data-stu-id="3bf73-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="3bf73-114">Lisätietoja on kohdassa [Laitteiden käyttöönotto](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="3bf73-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="3bf73-115">Luo DLP-käytäntöjä arkaluonteisten kohteiden suojaamiseksi.</span><span class="sxs-lookup"><span data-stu-id="3bf73-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="3bf73-116">Lisätietoja on kohdassa [Päätepisteen DLP-käytäntöjen skenaarioita](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="3bf73-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span></span>

<span data-ttu-id="3bf73-117">Lisätietoja Microsoftin päätepisteen DLP:stä on kohdassa [Microsoft 365:n päätepisteiden tietojen menetyksen estäminen (esikatselu)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="3bf73-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="3bf73-118">**Tärkeät tietojen keräysvaiheet, jos tukea tarvitaan:**</span><span class="sxs-lookup"><span data-stu-id="3bf73-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="3bf73-119">Lataa MDATP Client Analyzer Preview: [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span><span class="sxs-lookup"><span data-stu-id="3bf73-119">Download MDATP Client Analyzer Preview from [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="3bf73-120">Suorita työkalu järjestelmänvalvojana komentoikkunassa:</span><span class="sxs-lookup"><span data-stu-id="3bf73-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="3bf73-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="3bf73-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="3bf73-122">Kun näyttöön tulee kehote antaa seurantalokien keräämisen minuuttimäärä, syötä skenaarion suorittamiseen vaadittava minuuttimäärä.</span><span class="sxs-lookup"><span data-stu-id="3bf73-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="3bf73-123">Suorita skenaario</span><span class="sxs-lookup"><span data-stu-id="3bf73-123">Run the scenario</span></span>

<span data-ttu-id="3bf73-124">Ota talteen tukiedustajalle annettava zip-tiedosto.</span><span class="sxs-lookup"><span data-stu-id="3bf73-124">Collect the Zip file output to be given to the Support agent.</span></span>
