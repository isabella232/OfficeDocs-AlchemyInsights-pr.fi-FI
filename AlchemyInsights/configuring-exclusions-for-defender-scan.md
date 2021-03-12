---
title: Microsoft DefenderIN ATP-tarkistuksen poikkeusten määrittäminen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6027"
- "9001464"
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713572"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="fe9ad-102">Microsoft DefenderIN ATP-tarkistuksen poikkeusten määrittäminen</span><span class="sxs-lookup"><span data-stu-id="fe9ad-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="fe9ad-103">Yleensä voit jättää tietyt tiedostotunnisteet ja kansiosijainnit pois Microsoft Defender ATP -skannauksista.</span><span class="sxs-lookup"><span data-stu-id="fe9ad-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="fe9ad-104">Voit myös määrittää tiettyjen prosessien avaamia tiedostoja koskevat poikkeukset.</span><span class="sxs-lookup"><span data-stu-id="fe9ad-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="fe9ad-105">Lisätietoja [on](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) ruudussa Poikkeuksien määrittäminen ja vahvistaminen tiedostotunnisteen ja kansion sijainnin perusteella sekä prosessien avaamia tiedostoja [varten määritettyjen poikkeusten määrittäminen.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="fe9ad-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="fe9ad-106">Lisätietoja Windows **Server 2016:n ja 2019:n** poikkeusten määrittämisestä on kohdassa Microsoft Defenderin virustentorjunnan poikkeusten määrittäminen [Windows Serverissä.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="fe9ad-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="fe9ad-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="fe9ad-107">**Mac**</span></span>

<span data-ttu-id="fe9ad-108">Lisätietoja tuetuista poikkeustyypeistä ja poikkeusten luettelon määrittämisestä Macissa on ruudussa Tuetut poikkeustyypit ja Poikkeusten [luettelon määrittäminen.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions) [](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="fe9ad-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="fe9ad-109">**Huomautus** Voit myös tarkistaa poikkeusluettelot EICAR-testitiedoston avulla.</span><span class="sxs-lookup"><span data-stu-id="fe9ad-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="fe9ad-110">Lisätietoja on artikkelissa [Poikkeukset-luetteloiden vahvistaminen EICAR-testitiedoston avulla.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="fe9ad-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="fe9ad-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="fe9ad-111">**Linux**</span></span>

<span data-ttu-id="fe9ad-112">Lisätietoja tuetuista poikkeustyypeistä ja poissulkemisten luettelon [](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) määrittämisestä Linuxissa on ruudussa Tuetut poikkeustyypit sekä [Microsoft Defender ATP for Linuxin](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)poikkeusten määrittäminen ja vahvistaminen.</span><span class="sxs-lookup"><span data-stu-id="fe9ad-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="fe9ad-113">**Huomautus** Voit myös tarkistaa poikkeusluettelot EICAR-testitiedoston avulla.</span><span class="sxs-lookup"><span data-stu-id="fe9ad-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="fe9ad-114">Lisätietoja on artikkelissa [Poikkeukset-luetteloiden vahvistaminen EICAR-testitiedoston avulla.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="fe9ad-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 