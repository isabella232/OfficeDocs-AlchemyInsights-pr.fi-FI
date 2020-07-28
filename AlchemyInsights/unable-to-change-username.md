---
title: Käyttäjänimeä ei voi muuttaa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439552"
---
# <a name="unable-to-change-username"></a><span data-ttu-id="40ff3-102">Käyttäjänimeä ei voi muuttaa</span><span class="sxs-lookup"><span data-stu-id="40ff3-102">Unable to change UserName</span></span>

<span data-ttu-id="40ff3-103">Joissakin tapauksissa UPN (UserPrincipalName) -muutoksia ei välitetä pilveen.</span><span class="sxs-lookup"><span data-stu-id="40ff3-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="40ff3-104">Näyttöön saattaa tulla vahvistusvirheitä Office 365 -portaalissa tai et voi muuttaa käyttäjänimeä tai sähköpostiosoitetta.</span><span class="sxs-lookup"><span data-stu-id="40ff3-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="40ff3-105">Voit ratkaista tämän ongelman määrittämällä UserPrincipalName-nimen manuaalisesti käyttämällä tätä PowerShell-komentoa.</span><span class="sxs-lookup"><span data-stu-id="40ff3-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="40ff3-106">**Esimerkki: Käyttäjän nimeäminen uudelleen**</span><span class="sxs-lookup"><span data-stu-id="40ff3-106">**Example: Rename a user**</span></span>

<span data-ttu-id="40ff3-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="40ff3-107">PowerShellCopy</span></span>

<span data-ttu-id="40ff3-108">PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="40ff3-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="40ff3-109">Tämä komento nimeää davidc@contoso.com uudelleen davidchew@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="40ff3-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="40ff3-110">Lisätietoja on kohdassa [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span><span class="sxs-lookup"><span data-stu-id="40ff3-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>