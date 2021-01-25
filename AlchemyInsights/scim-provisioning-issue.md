---
title: SCIM-valmisteluongelma
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7854"
- "9004348"
ms.openlocfilehash: aa5b4cbb99cb1a5a323b39101766bea55fd49064
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949785"
---
# <a name="scim-provisioning-issue"></a><span data-ttu-id="fe34f-102">SCIM-valmisteluongelma</span><span class="sxs-lookup"><span data-stu-id="fe34f-102">SCIM provisioning issue</span></span>

<span data-ttu-id="fe34f-103">Automaattisella valmistelulla tarkoitetaan käyttäjien käyttäjänimien ja roolien luomista pilvisovelluksissa, joita käyttäjät tarvitsevat.</span><span class="sxs-lookup"><span data-stu-id="fe34f-103">Automatic provisioning refers to creating user identities and roles in the cloud applications that users need access to.</span></span> <span data-ttu-id="fe34f-104">Käyttäjäidentiteettien luomisen lisäksi automaattinen valmistelu sisältää käyttäjäidentiteettien ylläpidon ja poistamisen tilana tai roolien muuttuessa.</span><span class="sxs-lookup"><span data-stu-id="fe34f-104">In addition to creating user identities, automatic provisioning includes the maintenance and removal of user identities as status or roles change.</span></span> <span data-ttu-id="fe34f-105">Ennen kuin aloitat käyttöönoton, [](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) voit tarkistaa, miten valmistelu toimii, miten Azure Active Directory (AD) -valmistelu toimii, ja saada määrityssuosituksia.</span><span class="sxs-lookup"><span data-stu-id="fe34f-105">Before you start a deployment, you can review [How provisioning works](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) to learn how Azure Active Directory (AD) provision works, and get configuration recommendations.</span></span>

<span data-ttu-id="fe34f-106">Sovelluskehittäjänä voit käyttää System for Cross-Domain Identity Management (SCIM) -käyttäjähallinnan ohjelmointirajapintaa käyttäjien ja ryhmien automaattisen valmistelun mahdollistamiseksi sovelluksen ja Azure AD:n välillä.</span><span class="sxs-lookup"><span data-stu-id="fe34f-106">As an application developer, you can use the System for Cross-Domain Identity Management (SCIM) user management API to enable automatic provisioning of users and groups between your application and Azure AD.</span></span> <span data-ttu-id="fe34f-107">Voit [luoda SCIM-päätepisteen](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) ja määrittää käyttäjien valmistelun Azure AD:n artikkelin avulla. Tässä artikkelissa kerrotaan, miten VOIT LUODA SCIM-päätepisteen ja integroida sen Azure AD -valmistelupalveluun.</span><span class="sxs-lookup"><span data-stu-id="fe34f-107">The [Build a SCIM endpoint and configure user provisioning with Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) article describes how to build an SCIM endpoint and integrate it with the Azure AD provisioning service.</span></span>



