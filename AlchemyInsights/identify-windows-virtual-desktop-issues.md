---
title: Windowsin virtuaalityöpöydän ongelmien tunnistaminen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595628"
---
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="28328-102">Windowsin virtuaalityöpöydän ongelmien tunnistaminen</span><span class="sxs-lookup"><span data-stu-id="28328-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="28328-103">Windowsin virtuaalityöpöydän vianmääritys käyttää vain yhtä PowerShellin cmdlet-komentoa, mutta sisältää useita valinnaisia parametreja ongelmien rajaamista ja eristämista varten.</span><span class="sxs-lookup"><span data-stu-id="28328-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="28328-104">Aloittaminen:</span><span class="sxs-lookup"><span data-stu-id="28328-104">To get started:</span></span> 

1. <span data-ttu-id="28328-105">Lataa ja tuo Windows Virtual Desktop PowerShell -moduuli.</span><span class="sxs-lookup"><span data-stu-id="28328-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="28328-106">Lisätietoja on Windows [PowerShellin Windowsin virtuaalityöpöydän cmdlet-komennoissa.](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)</span><span class="sxs-lookup"><span data-stu-id="28328-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="28328-107">Kirjaudu tiliisi seuraavalla cmdlet-komennolla:</span><span class="sxs-lookup"><span data-stu-id="28328-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="28328-108">Esimerkki: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="28328-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="28328-109">**HUOMAUTUS:** Kaikissa PowerShellin kyselyissä on oltava joko -UserName- tai -ActivityID-parametrit.</span><span class="sxs-lookup"><span data-stu-id="28328-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="28328-110">Lisätietoja valvontaominaisuuksista on kohdassa [Lokianalyysin käyttäminen vianmääritystoimintoa varten.](https://go.microsoft.com/fwlink/?linkid=2126847)</span><span class="sxs-lookup"><span data-stu-id="28328-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="28328-111">Jos haluat suodattaa diagnostiikkatoiminnot käyttäjän mukaan, suorita seuraava cmdlet-komento:</span><span class="sxs-lookup"><span data-stu-id="28328-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="28328-112">Esimerkki: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="28328-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="28328-113">Voit suorittaa vianmääritykseen suodattimien luettelon.</span><span class="sxs-lookup"><span data-stu-id="28328-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="28328-114">Lisätietoja ongelmien selvittämiseksi on ohjeaiheessa Windowsin virtuaalityöpöydän ongelmien [tunnistaminen ja vianmääritys.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)</span><span class="sxs-lookup"><span data-stu-id="28328-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="28328-115">Lisätietoja yleisistä virheistä on kohdassa Yleiset [virheet senariot.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios)</span><span class="sxs-lookup"><span data-stu-id="28328-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
