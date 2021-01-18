---
title: Ryhmien määrittäminen Azure AD -rooliin
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885065"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="73524-102">Ryhmien määrittäminen Azure AD -rooliin</span><span class="sxs-lookup"><span data-stu-id="73524-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="73524-103">Voit määrittää Azure AD -ryhmän, jonka myöntäjä on Azure AD:ssä Azure AD -rooliin, toimimalla seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="73524-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="73524-104">Uuden ryhmän luominen – Uuden ryhmän luominen:</span><span class="sxs-lookup"><span data-stu-id="73524-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="73524-105">a.</span><span class="sxs-lookup"><span data-stu-id="73524-105">a.</span></span> <span data-ttu-id="73524-106">Kirjaudu Azure AD -hallintakeskukseen järjestelmänvalvojan **tai** yleisen **järjestelmänvalvojan** käyttöoikeuksilla.</span><span class="sxs-lookup"><span data-stu-id="73524-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="73524-107">b.</span><span class="sxs-lookup"><span data-stu-id="73524-107">b.</span></span> <span data-ttu-id="73524-108">Valitse **Azure Active Directory > ryhmät > Kaikki ryhmät > uusi ryhmä**.</span><span class="sxs-lookup"><span data-stu-id="73524-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="73524-109">c.</span><span class="sxs-lookup"><span data-stu-id="73524-109">c.</span></span> <span data-ttu-id="73524-110">Luo ryhmä.</span><span class="sxs-lookup"><span data-stu-id="73524-110">Create the group.</span></span>

2. <span data-ttu-id="73524-111">Määritä ryhmälle rooli joko ryhmän luomisen tai sen luomisen jälkeen.</span><span class="sxs-lookup"><span data-stu-id="73524-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="73524-112">a.</span><span class="sxs-lookup"><span data-stu-id="73524-112">a.</span></span> <span data-ttu-id="73524-113">Jos haluat määrittää ryhmälle roolin ryhmän luomisen yhteydessä, voit määrittää ryhmälle **azure AD** -roolien vaihtopainikkeen ja luoda ryhmän.</span><span class="sxs-lookup"><span data-stu-id="73524-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="73524-114">b.</span><span class="sxs-lookup"><span data-stu-id="73524-114">b.</span></span> <span data-ttu-id="73524-115">Jos haluat määrittää roolin ryhmälle sen luomisen  jälkeen, siirry juuri luodun ryhmän Määritetyt roolit -välilehteen ja määritä rooli ryhmälle.</span><span class="sxs-lookup"><span data-stu-id="73524-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="73524-116">**Azure AD -rooliin määritetyn ryhmän jäsenyyden hallinta**</span><span class="sxs-lookup"><span data-stu-id="73524-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="73524-117">Oletusarvoisesti vain järjestelmänvalvojat ja yleiset järjestelmänvalvojat voivat estää oikeuksien laajentamisen muokkaamalla rooliin määritetyn ryhmän jäsenyyttä.</span><span class="sxs-lookup"><span data-stu-id="73524-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="73524-118">He voivat kuitenkin määrittää omistajalle tällaisen ryhmän ja delegoida tämän tehtävän.</span><span class="sxs-lookup"><span data-stu-id="73524-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="73524-119">Lisätietoja pilviryhmien määrittämisestä Azure AD -rooleille on kohdassa AD-roolien [määrittäminen pilviryhmälle.](https://docs.microsoft.com/azure/active-directory/roles/groups-concept)</span><span class="sxs-lookup"><span data-stu-id="73524-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="73524-120">Lisätietoja pilviryhmille määritettyjen roolien vianmäärityksestä on kohdassa [Pilviryhmille määritettyjen roolien vianmääritys.](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="73524-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





