---
title: DKIM:n ottaminen käyttöön tietyssä toimialueella Exchange Online PowerShellin avulla
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524173"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a><span data-ttu-id="4b088-102">DKIM:n ottaminen käyttöön tietyssä toimialueella Exchange Online PowerShellin avulla</span><span class="sxs-lookup"><span data-stu-id="4b088-102">Use Exchange Online PowerShell to enable DKIM for a specific domain</span></span>

<span data-ttu-id="4b088-103">Jos et voi luoda DKIM DNS -tietueita hallintakeskuksessa, kokeile Exchange Online PowerShelliä.</span><span class="sxs-lookup"><span data-stu-id="4b088-103">If you can't create the DKIM DNS records in the admin center, try using Exchange Online PowerShell.</span></span> 

<span data-ttu-id="4b088-104">Voit luoda DKIM DNS -tietueen Exchange Online PowerShellin avulla seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="4b088-104">To create a DKIM DNS record using Exchange Online PowerShell, perform the following steps:</span></span>

1. <span data-ttu-id="4b088-105">Avaa Windows PowerShell järjestelmänvalvojana ja suorita seuraavat komennot seuraavassa järjestyksessä:</span><span class="sxs-lookup"><span data-stu-id="4b088-105">Open Windows PowerShell as an administrator and run the following commands in the described sequence:</span></span>

    <span data-ttu-id="4b088-106">a.</span><span class="sxs-lookup"><span data-stu-id="4b088-106">a.</span></span> `$UserCredential = Get-Credential`

    <span data-ttu-id="4b088-107">b.</span><span class="sxs-lookup"><span data-stu-id="4b088-107">b.</span></span> `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="4b088-108">c.</span><span class="sxs-lookup"><span data-stu-id="4b088-108">c.</span></span> `Import-PSSession $Session -DisableNameChecking`
    
<span data-ttu-id="4b088-109">Jos sinulla on ongelmia yhteyden muodostamisessa Exchange Online PowerShelliin, katso [kohta Yhteyden muodostaminen Exchange Online PowerShelliin.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)</span><span class="sxs-lookup"><span data-stu-id="4b088-109">If you have trouble connecting to Exchange Online PowerShell, see [Connect to Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="4b088-110">Kun olet muodostanut yhteyden Exchange Online PowerShelliin, suorita seuraava komento:</span><span class="sxs-lookup"><span data-stu-id="4b088-110">Once you're connected to Exchange Online PowerShell, run the following command:</span></span>

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. <span data-ttu-id="4b088-111">Kun yllä oleva komento on suoritettu onnistuneesti, lopeta Exchange Online PowerShell -istunto suorittamalla seuraava komento:</span><span class="sxs-lookup"><span data-stu-id="4b088-111">Once the above command has been successfully executed, run the following command to terminate the Exchange Online PowerShell session:</span></span>

    `Remove-PSSession $Session` 



