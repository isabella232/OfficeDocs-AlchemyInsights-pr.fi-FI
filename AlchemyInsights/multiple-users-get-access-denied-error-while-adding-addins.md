---
title: Useat käyttäjät saavat käyttö estetty -virheen lisättäessä apuosia Outlookissa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423712"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="050cb-102">Useat käyttäjät saavat käyttö estetty -virheen lisättäessä apuosia Outlookissa</span><span class="sxs-lookup"><span data-stu-id="050cb-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="050cb-103">Voit määrittää, kenellä organisaation järjestelmänvalvojilla on oikeudet asentaa ja hallita Outlookin apuohjelmia.</span><span class="sxs-lookup"><span data-stu-id="050cb-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="050cb-104">Voit myös määrittää, kenellä organisaation käyttäjillä on oikeus asentaa ja hallita apuohjelmia omaan käyttöönsä.</span><span class="sxs-lookup"><span data-stu-id="050cb-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="050cb-105">Lisätietoja on [ohjeaiheessa Outlookin apuohjelmia asentavien ja hallitsevien järjestelmänvalvojien ja käyttäjien määrittäminen](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="050cb-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="050cb-106">Voit varmistaa, että olet määrittänyt käyttöoikeudet käyttäjälle, <Role Name> korvaamalla tarkistettavan roolin nimen ja suorittamalla seuraavan komennon Exchange Online PowerShellissä:</span><span class="sxs-lookup"><span data-stu-id="050cb-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="050cb-107">Get-ManagementRoleAssignment -Rooli " <Role Name> " -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="050cb-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="050cb-108">Tässä esimerkissä kerrotaan, miten voit tarkistaa, kenelle olet määrittänyt käyttöoikeudet apuosten asentamiseen organisaation Office-kaupasta.</span><span class="sxs-lookup"><span data-stu-id="050cb-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="050cb-109">Powershell</span><span class="sxs-lookup"><span data-stu-id="050cb-109">PowerShell</span></span>

<span data-ttu-id="050cb-110">-Rooli "Org Marketplace Apps" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="050cb-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="050cb-111">Tarkista tulokset Get-ManagementRoleAssignment, Tarkista Tehokkaat käyttäjät -sarakkeen merkinnät.</span><span class="sxs-lookup"><span data-stu-id="050cb-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="050cb-112">Yksityiskohtaiset syntaksi- ja parametritiedot ovat kohdassa [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="050cb-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 