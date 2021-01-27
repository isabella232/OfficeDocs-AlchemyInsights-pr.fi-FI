---
title: Sovellusten poistaminen tai palauttaminen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014799"
---
# <a name="delete-or-restore-applications"></a><span data-ttu-id="a773e-102">Sovellusten poistaminen tai palauttaminen</span><span class="sxs-lookup"><span data-stu-id="a773e-102">Delete or restore applications</span></span>

<span data-ttu-id="a773e-103">**Sovelluksen poistaminen Azure AD -vuokraajassa:**</span><span class="sxs-lookup"><span data-stu-id="a773e-103">**To delete an application from your Azure AD tenant**:</span></span>

1. <span data-ttu-id="a773e-104">Valitse **Azure AD -portaalissa** **Yrityssovellukset.**</span><span class="sxs-lookup"><span data-stu-id="a773e-104">In the **Azure AD portal**, select **Enterprise applications**.</span></span> <span data-ttu-id="a773e-105">Etsi ja valitse sitten sovellus, jonka haluat poistaa.</span><span class="sxs-lookup"><span data-stu-id="a773e-105">Then find and select the application you want to delete.</span></span>
2. <span data-ttu-id="a773e-106">Valitse **vasemmanpuoleisen** ruudun Hallinta-osassa **Ominaisuudet.**</span><span class="sxs-lookup"><span data-stu-id="a773e-106">In the **Manage** section in the left pane, select **Properties**.</span></span>
3. <span data-ttu-id="a773e-107">Vahvista **sovelluksen** poistaminen  Azure AD -vuokraajassa valitsemalla Poista ja valitsemalla sitten Kyllä.</span><span class="sxs-lookup"><span data-stu-id="a773e-107">Select **Delete**, and then select **Yes** to confirm you want to delete the app from your Azure AD tenant.</span></span>

<span data-ttu-id="a773e-108">Lisätietoja sovelluksen poistosta on pika-aloitustoiminn kohdassa: Sovelluksen poistaminen [Azure Active Directory (Azure AD) -vuokraajassa.](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)</span><span class="sxs-lookup"><span data-stu-id="a773e-108">For more information on how to delete an app, see [Quickstart: Delete an application from your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span></span>

<span data-ttu-id="a773e-109">[PowerShellissä Remove-AzureADApplicationProxyApplication-cmdlet-komento](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) poistaa sovelluksen välityspalvelimen määritykset tietystä Azure Active Directoryn sovelluksesta ja voi poistaa sovelluksen kokonaan, jos se on määritetty.</span><span class="sxs-lookup"><span data-stu-id="a773e-109">In PowerShell, the [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet removes Application Proxy configurations from a specific application in Azure Active Directory, and can delete the application completely if specified.</span></span>

<span data-ttu-id="a773e-110">Voit palauttaa **poistetun sovelluksen** PowerShellin avulla.</span><span class="sxs-lookup"><span data-stu-id="a773e-110">You can **restore a deleted application** using PowerShell.</span></span> <span data-ttu-id="a773e-111">Kun palautettava sovellus on tunnistettu, voit palauttaa sen [Restore-AzureADDeletedApplication-sovelluksella.](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)</span><span class="sxs-lookup"><span data-stu-id="a773e-111">Once the application you want to restore has been identified, you can restore it using [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span></span>
