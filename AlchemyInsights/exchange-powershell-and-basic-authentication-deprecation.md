---
title: Exchange PowerShell ja perustodentamisen käytöstä poistuminen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015686"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="7b71a-102">Exchange PowerShell ja perustodentamisen käytöstä poistuminen</span><span class="sxs-lookup"><span data-stu-id="7b71a-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="7b71a-103">Jos haluat lisätietoja yhteyden muodostamisesta Exchange Online PowerShelliin ilman perustodentamista, [siirry tänne](https://aka.ms/psbasicauth).</span><span class="sxs-lookup"><span data-stu-id="7b71a-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/psbasicauth).</span></span>

<span data-ttu-id="7b71a-104">Ota huomioon, että asiakaskoneessa on yhä otettava käyttöön perustodennus.</span><span class="sxs-lookup"><span data-stu-id="7b71a-104">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="7b71a-105">Uusi PowerShell V2 -moduuli käyttää modernia todennusta yhteyden luomiseen, jotta kaikki REST-pohjaiset V2 cmdlet -komennot voidaan ottaa käyttöön.</span><span class="sxs-lookup"><span data-stu-id="7b71a-105">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="7b71a-106">V2 cmdlet -komentojen lisäksi voit käyttää sen avulla vanhemman etä-PowerShellin (RPS) cmdlet-komentoja, jotka edellyttävät etä-PowerShell-istuntoa.</span><span class="sxs-lookup"><span data-stu-id="7b71a-106">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="7b71a-107">RPS-istunnon luominen Windows-tietokoneessa edellyttää, että WinRM-perustodennus on käytössä asiakaskoneessa, vaikka moduuli käyttää modernia todennusmekanismia palvelun todentamiseen.</span><span class="sxs-lookup"><span data-stu-id="7b71a-107">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="7b71a-108">WinRM-perustodennusjaksoa käytetään modernien todennustunnusten siirtämiseen.</span><span class="sxs-lookup"><span data-stu-id="7b71a-108">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="7b71a-109">Jos WinRM-perustodennus ei ole käytössä asiakaskoneessa, uudet V2 cmdlet -komennot toimivat (mutta vanhemmat RPS cmdlet -komennot eivät).</span><span class="sxs-lookup"><span data-stu-id="7b71a-109">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
