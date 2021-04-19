---
title: Exchange PowerShell ja perustodentamisen käytöstä poistuminen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813469"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="d0ecd-102">Exchange PowerShell ja perustodentamisen käytöstä poistuminen</span><span class="sxs-lookup"><span data-stu-id="d0ecd-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="d0ecd-103">Jos haluat lisätietoja yhteyden muodostamisesta Exchange Online PowerShelliin ilman perustodentamista, [siirry tänne](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="d0ecd-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="d0ecd-104">PowerShell V2 -moduuli ei käytä perustodennusta.</span><span class="sxs-lookup"><span data-stu-id="d0ecd-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="d0ecd-105">Ota huomioon, että asiakaskoneessa on yhä otettava käyttöön perustodennus.</span><span class="sxs-lookup"><span data-stu-id="d0ecd-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="d0ecd-106">Uusi PowerShell V2 -moduuli käyttää modernia todennusta yhteyden luomiseen, jotta kaikki REST-pohjaiset V2 cmdlet -komennot voidaan ottaa käyttöön.</span><span class="sxs-lookup"><span data-stu-id="d0ecd-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="d0ecd-107">V2 cmdlet -komentojen lisäksi voit käyttää sen avulla vanhemman etä-PowerShellin (RPS) cmdlet-komentoja, jotka edellyttävät etä-PowerShell-istuntoa.</span><span class="sxs-lookup"><span data-stu-id="d0ecd-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="d0ecd-108">RPS-istunnon luominen Windows-tietokoneessa edellyttää, että WinRM-perustodennus on käytössä asiakaskoneessa, vaikka moduuli käyttää modernia todennusmekanismia palvelun todentamiseen.</span><span class="sxs-lookup"><span data-stu-id="d0ecd-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="d0ecd-109">WinRM-perustodennusjaksoa käytetään modernien todennustunnusten siirtämiseen.</span><span class="sxs-lookup"><span data-stu-id="d0ecd-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="d0ecd-110">Jos WinRM-perustodennus ei ole käytössä asiakaskoneessa, uudet V2 cmdlet -komennot toimivat (mutta vanhemmat RPS cmdlet -komennot eivät).</span><span class="sxs-lookup"><span data-stu-id="d0ecd-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
