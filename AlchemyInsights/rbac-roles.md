---
title: 'RBAC-roolit '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583544"
---
# <a name="rbac-rules"></a><span data-ttu-id="f88f8-102">RBAC-säännöt</span><span class="sxs-lookup"><span data-stu-id="f88f8-102">RBAC rules</span></span>

<span data-ttu-id="f88f8-103">Jos saat käyttö oikeus virheen, toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="f88f8-103">If you get the permission error:</span></span> 

- <span data-ttu-id="f88f8-104">**Asiakkaalla, jolla on objekti tunnus, ei ole valtuutusta suorittaa toimenpiteitä vaikutus alueen kautta (koodi: Authorizatiepäonnistui)**: kun yrität luoda resurssin, tarkista, että olet kirjautuneena sellaisen käyttäjän kanssa, jolle on määritetty rooli, jolla on kirjoitus oikeudet valittuun käyttö alueen resurssiin.</span><span class="sxs-lookup"><span data-stu-id="f88f8-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="f88f8-105">Jos haluat esimerkiksi hallita näennäiskoneita resurssi ryhmässä, sinulla pitäisi olla [näennäiskoneen avustaja](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) -rooli resurssi ryhmässä (tai pääkäyttö alue).</span><span class="sxs-lookup"><span data-stu-id="f88f8-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="f88f8-106">Luettelo kunkin sisäisen roolin käyttö oikeuksista on kohdassa [Azure-resurssien sisäiset roolit](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="f88f8-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="f88f8-107">**Sinulla ei ole oikeutta luoda tuki pyyntöä**: kun yrität luoda tai päivittää tuki lippua, tarkista, että olet kirjautuneena käyttäjänä, jolle on määritetty rooli, jossa on Microsoft. support/supportTickets/Write-oikeus, kuten [tuki pyynnön avustaja](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span><span class="sxs-lookup"><span data-stu-id="f88f8-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="f88f8-108">**Rooli määrityksiä ei voi luoda enempää (koodi: Roleassignmentlimitetceeded)**: kun yrität määrittää roolia, yritä vähentää rooli varausten määrää määrittämällä rooleja ryhmille.</span><span class="sxs-lookup"><span data-stu-id="f88f8-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="f88f8-109">Azure tukee enintään **2000** -rooli määritystä pakettikohtaisesti.</span><span class="sxs-lookup"><span data-stu-id="f88f8-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="f88f8-110">Lisä tietoja Azure RBAC-rooleista on Ohje aiheessa [Azure RBAC-roolit](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="f88f8-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
