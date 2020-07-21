---
title: Orpokäyttäjän poistaminen paikallisesta palvelimesta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198185"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="d3dba-102">Orpokäyttäjän poistaminen paikallisesta palvelimesta</span><span class="sxs-lookup"><span data-stu-id="d3dba-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="d3dba-103">Voit poistaa orpokäyttäjän seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="d3dba-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="d3dba-104">Pakota hakemistosynkronointi noudattamalla kohdassa [Mikä on yhdistelmäkäyttäjätieto Azure Active Directoryssa?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span><span class="sxs-lookup"><span data-stu-id="d3dba-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="d3dba-105">Lisätietoja hakemistosynkronoinnin tarkistamisesta [on ohjeaiheessa Mikä on azure Active Directoryn yhdistelmäkäyttäjän tunnus?](https://technet.microsoft.com/library/jj151797.aspx).</span><span class="sxs-lookup"><span data-stu-id="d3dba-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="d3dba-106">Jos synkronointi toimii oikein, mutta Active Directory -objektin poistaminen ei toimi Azure AD:hen, poista orpoobjekti manuaalisesti jollakin seuraavista Azure Active Directory -moduulin käyttämisestä Windows PowerShell -cmdlet-komentoja varten:</span><span class="sxs-lookup"><span data-stu-id="d3dba-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="d3dba-107">Poista-MsolContact</span><span class="sxs-lookup"><span data-stu-id="d3dba-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="d3dba-108">Poista MsolGroup</span><span class="sxs-lookup"><span data-stu-id="d3dba-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="d3dba-109">Poista-MsolUser</span><span class="sxs-lookup"><span data-stu-id="d3dba-109">Remove-MsolUser</span></span>

    <span data-ttu-id="d3dba-110">Jos esimerkiksi haluat poistaa orpoja käyttäjätunnuksia john.smith@contoso.com, joka on alun perin luotu hakemistosynkronoinnin avulla, suorita cmdlet-komento:</span><span class="sxs-lookup"><span data-stu-id="d3dba-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="d3dba-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="d3dba-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>