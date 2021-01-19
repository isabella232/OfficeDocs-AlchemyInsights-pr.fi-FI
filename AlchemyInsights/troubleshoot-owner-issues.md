---
title: Omistajan ongelmien vianmääritys
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7815"
- "9004358"
ms.openlocfilehash: 914d5682a403197a8569bb75fda8a77449f485f6
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901007"
---
# <a name="troubleshoot-owner-issues"></a><span data-ttu-id="b8833-102">Omistajan ongelmien vianmääritys</span><span class="sxs-lookup"><span data-stu-id="b8833-102">Troubleshoot owner issues</span></span>

<span data-ttu-id="b8833-103">Voit tehdä omistajan ongelmien vianmäärityksen seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="b8833-103">To troubleshoot owner-related issues, perform the following steps:</span></span>

1. <span data-ttu-id="b8833-104">[Azure-tilauksen järjestelmänvalvojien lisääminen](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners)tai muuttaminen: Azure Active Directory (Azure AD) -ryhmät ovat ryhmien omistamia ja hallinnoimia.</span><span class="sxs-lookup"><span data-stu-id="b8833-104">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): Azure Active Directory (Azure AD) groups are owned and managed by group owners.</span></span> <span data-ttu-id="b8833-105">Ryhmän omistajat voivat olla käyttäjiä tai palvelun pääkäyttäjiä, ja he voivat hallita ryhmää, myös jäsenyyttä.</span><span class="sxs-lookup"><span data-stu-id="b8833-105">Group owners can be users or service principals, and are able to manage the group, including membership.</span></span> <span data-ttu-id="b8833-106">Vain olemassa olevat ryhmän omistajat tai ryhmän hallinnoijat voivat määrittää ryhmän omistajia.</span><span class="sxs-lookup"><span data-stu-id="b8833-106">Only existing group owners or group-managing administrators can assign group owners.</span></span> <span data-ttu-id="b8833-107">Ryhmän omistajien ei tarvitse olla ryhmän jäseniä.</span><span class="sxs-lookup"><span data-stu-id="b8833-107">Group owners aren't required to be members of the group.</span></span>
2. <span data-ttu-id="b8833-108">[Azure-tilauksen järjestelmänvalvojien](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)lisääminen tai muuttaminen: Tässä artikkelissa kerrotaan, miten voit lisätä tai muuttaa järjestelmänvalvojan roolia käyttäjälle, joka käyttää Azure RBAC:tä tilausalueen mukaisesti.</span><span class="sxs-lookup"><span data-stu-id="b8833-108">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): This article describes how to add or change the administrator role for a user using Azure RBAC at the subscription scope.</span></span>
3. <span data-ttu-id="b8833-109">PowerShellin avulla voit lisätä ryhmän omistajan tai sovelluksen omistajan.</span><span class="sxs-lookup"><span data-stu-id="b8833-109">Use PowerShell to add a group owner or an application owner.</span></span>
