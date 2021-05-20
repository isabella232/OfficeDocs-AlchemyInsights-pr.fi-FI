---
title: Poikkeuksien määrittäminen Microsoft Defender ATP tarkistamista varten
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
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543682"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="e11c3-102">Poikkeuksien määrittäminen Microsoft Defender ATP tarkistamista varten</span><span class="sxs-lookup"><span data-stu-id="e11c3-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="e11c3-103">Yleensä voit jättää tietyt tiedostotunnisteet ja kansiosijainnit pois Microsoft Defender ATP tarkistamuksista.</span><span class="sxs-lookup"><span data-stu-id="e11c3-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="e11c3-104">Voit myös määrittää tiettyjen prosessien avaamia tiedostoja koskevat poikkeukset.</span><span class="sxs-lookup"><span data-stu-id="e11c3-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="e11c3-105">Lisätietoja [on](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) ruuduissa Poikkeuksien määrittäminen ja vahvistaminen tiedostotunnisteen ja kansion sijainnin perusteella ja [Prosessien avaamia tiedostoja koskevat poikkeusten määrittäminen.](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="e11c3-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="e11c3-106">Lisätietoja **Windows Server 2016:n ja 2019:n** poikkeusten määrittämisestä on Microsoft Defenderin virustentorjunta [poikkeuksien Windows palvelimessa.](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="e11c3-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="e11c3-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="e11c3-107">**Mac**</span></span>

<span data-ttu-id="e11c3-108">Lisätietoja tuetuista poikkeustyypeistä ja poikkeusluettelon määrittämisestä [](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) Macissa on ruudussa Tuetut poikkeustyypit ja [Poissulkemisluettelon määrittäminen.](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions)</span><span class="sxs-lookup"><span data-stu-id="e11c3-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="e11c3-109">**Huomautus** Voit myös tarkistaa poikkeusluettelot EICAR-testitiedoston avulla.</span><span class="sxs-lookup"><span data-stu-id="e11c3-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="e11c3-110">Lisätietoja on artikkelissa Poikkeusten [luetteloiden vahvistaminen EICAR-testitiedostolla.](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="e11c3-110">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="e11c3-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="e11c3-111">**Linux**</span></span>

<span data-ttu-id="e11c3-112">Lisätietoja tuetuista poissulkemistyypeistä ja poissulkemisluettelon [](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) määrittämisestä Linuxissa on ruuduissa Tuetut poikkeustyypit ja [Microsoft Defender ATP:n ohitustyyppien määrittäminen ja vahvistaminen.](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="e11c3-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="e11c3-113">**Huomautus** Voit myös tarkistaa poikkeusluettelot EICAR-testitiedoston avulla.</span><span class="sxs-lookup"><span data-stu-id="e11c3-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="e11c3-114">Lisätietoja on artikkelissa Poikkeusten [luetteloiden vahvistaminen EICAR-testitiedostolla.](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="e11c3-114">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 