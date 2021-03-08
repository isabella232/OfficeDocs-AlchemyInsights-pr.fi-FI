---
title: Aseta ClientAccessServerEnabled-arvoksi Tosi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524558"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="75a98-102">Aseta ClientAccessServerEnabled-arvoksi Tosi</span><span class="sxs-lookup"><span data-stu-id="75a98-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="75a98-103">Jos et voi avata salattua sähköpostiviestiä ja nähdä sen sijaan **rpmsg-liitteen,** toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="75a98-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="75a98-104">Muodosta yhteys Exchange Online PowerShelliin.</span><span class="sxs-lookup"><span data-stu-id="75a98-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="75a98-105">Jos haluat muodostaa yhteyden Exchange Online PowerShelliin, sinun on kirjauduttava sisään yleisen järjestelmänvalvojan tai Exchange-järjestelmänvalvojan tilillä.</span><span class="sxs-lookup"><span data-stu-id="75a98-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="75a98-106">a.</span><span class="sxs-lookup"><span data-stu-id="75a98-106">a.</span></span> <span data-ttu-id="75a98-107">Avaa Windows PowerShell ja suorita sitten seuraava komento: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="75a98-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="75a98-108">b.</span><span class="sxs-lookup"><span data-stu-id="75a98-108">b.</span></span> <span data-ttu-id="75a98-109">Kirjoita **Windows PowerShellin tunnistetietopyyntö** -valintaikkunaan työ- tai koulutilisi ja salasanasi, c.</span><span class="sxs-lookup"><span data-stu-id="75a98-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="75a98-110">Valitse **OK**.</span><span class="sxs-lookup"><span data-stu-id="75a98-110">Click **OK**.</span></span> 

2. <span data-ttu-id="75a98-111">Luo uusi istunto suoritamalla seuraava komento:</span><span class="sxs-lookup"><span data-stu-id="75a98-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="75a98-112">a.</span><span class="sxs-lookup"><span data-stu-id="75a98-112">a.</span></span> <span data-ttu-id="75a98-113">Suorita seuraava komento:</span><span class="sxs-lookup"><span data-stu-id="75a98-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="75a98-114">`Get-IRMConfiguration`Suorita-komento.</span><span class="sxs-lookup"><span data-stu-id="75a98-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="75a98-115">Tarkista **ClientAccessServerEnabled-asetus.**</span><span class="sxs-lookup"><span data-stu-id="75a98-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="75a98-116">a.</span><span class="sxs-lookup"><span data-stu-id="75a98-116">a.</span></span> <span data-ttu-id="75a98-117">Jos **ClientAccessServerEnabled-asetuksena** on **Epätosi,** suorita seuraava cmdlet-komento: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="75a98-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="75a98-118">Sulje powershell-istunto aina seuraavalla komennolla: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="75a98-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="75a98-119">Lisätietoja on Exchange [Online PowerShellissä.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)</span><span class="sxs-lookup"><span data-stu-id="75a98-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

