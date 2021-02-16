---
title: Ryhmän synkronointi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256718"
---
# <a name="group-sync"></a><span data-ttu-id="49fa2-102">Ryhmän synkronointi</span><span class="sxs-lookup"><span data-stu-id="49fa2-102">Group sync</span></span>

<span data-ttu-id="49fa2-103">Tässä artikkelissa on ryhmän synkronointia koskevat ohjeet.</span><span class="sxs-lookup"><span data-stu-id="49fa2-103">This article provides guidance on group synchronization.</span></span>

1. <span data-ttu-id="49fa2-104">Jos yleinen järjestelmänvalvoja tai ryhmän omistaja ei voi muokata ryhmän ominaisuuksia tai lisätä jäseniä tai määrittää omistajia Azure-portaalissa, varmista, että ryhmän myöntäjän lähde on Azure Active Directory (Azure AD), jotta yleinen järjestelmänvalvoja tai ryhmän omistaja voi muokata ryhmää.</span><span class="sxs-lookup"><span data-stu-id="49fa2-104">If a global admin or group owner is not able to modify group properties or add members or assign owners in the Azure portal, ensure the source of the authority for the group is Azure Active Directory (Azure AD) for the global admin or group owner to modify the group.</span></span>
2. <span data-ttu-id="49fa2-105">Ennen kuin yrität poistaa synkronoidun ryhmän Azure [AD:ssä,](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) varmista, että olet poistanut kaikki määritetyt käyttöoikeudet virheiden välttämiseksi.</span><span class="sxs-lookup"><span data-stu-id="49fa2-105">Before attempting to delete a synced group in Azure AD, ensure you have [deleted all assigned licenses](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) to avoid errors.</span></span>

<span data-ttu-id="49fa2-106">Lisätietoja käyttäjien, ryhmien ja yhteystietojen synkronoinnista on Azure AD Connect -synkronoinnissa ja paikallisen ryhmän synkronoinnin seuraaminen [Azure AD Connectin](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) avulla perm-ryhmien synkronoimiseksi AD Connectin avulla. [](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts)</span><span class="sxs-lookup"><span data-stu-id="49fa2-106">For understanding how to sync users, groups and contacts, see [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), and follow [Syncing an on-premises group to Azure using Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) to sync on-perm groups using AD connect.</span></span>

<span data-ttu-id="49fa2-107">Suorita synkronoinnin [aikana yleisimpiä virheitä](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) vianmääritystä varten tämän oppaan ohjeiden mukaisesti.</span><span class="sxs-lookup"><span data-stu-id="49fa2-107">Follow this guide [Troubleshooting Errors during synchronization](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) to troubleshoot common errors during synchronization.</span></span>

