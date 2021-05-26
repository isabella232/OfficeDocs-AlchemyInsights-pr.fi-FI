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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657926"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="8fe28-102">Määritä päätepisteen DLP</span><span class="sxs-lookup"><span data-stu-id="8fe28-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="8fe28-103">Microsoftin päätepisteen DLP sallii sinun laajentaa tietojen menetyksen estämisen suojausta ja arkaluonteisten tietojen valvontakykyä Windows 10 -laitteissa.</span><span class="sxs-lookup"><span data-stu-id="8fe28-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="8fe28-104">Kun laitteet on otettu käyttöön laitteiden hallinnassa, voit luoda DLP-käytäntöjä kohteiden suojaustoimiin.</span><span class="sxs-lookup"><span data-stu-id="8fe28-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="8fe28-105">Toiminnan hallinnassa voit valvoa arkaluonteisten kohteiden toimintaa.</span><span class="sxs-lookup"><span data-stu-id="8fe28-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="8fe28-106">Lisätietoja on kohdassa [Laitteiden käyttöönotto laitteiden hallinnassa](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="8fe28-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="8fe28-107">Jos haluat aloittaa päätepisteen DLP:n käytön:</span><span class="sxs-lookup"><span data-stu-id="8fe28-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="8fe28-108">Varmista, että sinulla on tarvittavat SKU- tai tilauskäyttöoikeudet.</span><span class="sxs-lookup"><span data-stu-id="8fe28-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="8fe28-109">Lisätietoja on kohdassa [SKU- tai tilauskäyttöoikeudet](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="8fe28-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="8fe28-110">Tarkista käyttöoikeudet, jotka vaaditaan laitteiden hallintaan, laitteiden lisäyssivulle pääsyyn tai laitteiden valvonnan käyttöönottoon tai sen käytöstä poistamiseen.</span><span class="sxs-lookup"><span data-stu-id="8fe28-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="8fe28-111">Lisätietoja on kohdassa [Käyttöoikeudet](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="8fe28-111">For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="8fe28-112">Lisää laitteita laitteiden hallintaan noudattamalla laitteiden käyttöönoton toimintosarjaa.</span><span class="sxs-lookup"><span data-stu-id="8fe28-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="8fe28-113">Lisätietoja on kohdassa [Laitteiden käyttöönotto](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="8fe28-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="8fe28-114">Luo DLP-käytäntöjä arkaluonteisten kohteiden suojaamiseksi.</span><span class="sxs-lookup"><span data-stu-id="8fe28-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="8fe28-115">Lisätietoja on kohdassa [Päätepisteen DLP-käytäntöjen skenaarioita](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="8fe28-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="8fe28-116">Lisätietoja Microsoftin päätepisteen DLP:stä on kohdassa [Microsoft 365:n päätepisteiden tietojen menetyksen estäminen (esikatselu)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="8fe28-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="8fe28-117">**Tärkeät tietojen keräysvaiheet, jos tukea tarvitaan:**</span><span class="sxs-lookup"><span data-stu-id="8fe28-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="8fe28-118">Lataa [MDATP Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span><span class="sxs-lookup"><span data-stu-id="8fe28-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="8fe28-119">Suorita työkalu järjestelmänvalvojana komentoikkunassa:</span><span class="sxs-lookup"><span data-stu-id="8fe28-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="8fe28-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="8fe28-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="8fe28-121">Kun näyttöön **tulee Anna seurantalokien keräämiseen tarvittava minuuttimäärä:**, kirjoita skenaarion suorittamiseen tarvittava minuuttimäärä.</span><span class="sxs-lookup"><span data-stu-id="8fe28-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="8fe28-122">Suorita skenaario.</span><span class="sxs-lookup"><span data-stu-id="8fe28-122">Run the scenario.</span></span>

<span data-ttu-id="8fe28-123">Kerää Zip-tiedoston tuloste tukiedustajalle annettavaksi.</span><span class="sxs-lookup"><span data-stu-id="8fe28-123">Collect the Zip file output to give to the Support agent.</span></span>
