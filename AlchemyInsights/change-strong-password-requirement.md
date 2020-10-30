---
title: Vahvan salasana vaatimuksen muuttaminen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 8ce331275e066b5a4f177ae27178ec726f90762f
ms.sourcegitcommit: aa35d2e1829f7d07f64fb891bf73b1fd80f0864c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/30/2020
ms.locfileid: "48804420"
---
# <a name="change-strong-password-requirement"></a><span data-ttu-id="386a8-102">Vahvan salasana vaatimuksen muuttaminen</span><span class="sxs-lookup"><span data-stu-id="386a8-102">Change strong password requirement</span></span>

<span data-ttu-id="386a8-103">Microsoft vaatii oletusarvoisesti vahvat Sala sanat.</span><span class="sxs-lookup"><span data-stu-id="386a8-103">Microsoft requires strong passwords by default.</span></span>

<span data-ttu-id="386a8-104">PowerShellin avulla voit poistaa käytöstä tiettyjen käyttäjien vahvat Sala sanat seuraavilla komennoilla:</span><span class="sxs-lookup"><span data-stu-id="386a8-104">Using PowerShell, you can disable strong passwords for specific users with these commands:</span></span>

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

<span data-ttu-id="386a8-105">Jos haluat poistaa käytöstä kaikkien käyttäjien vahvat Sala sanat, käytä:</span><span class="sxs-lookup"><span data-stu-id="386a8-105">To disable strong passwords for all users, use:</span></span>

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [<span data-ttu-id="386a8-106">Lisä tietoja salasana käytännöstä</span><span class="sxs-lookup"><span data-stu-id="386a8-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="386a8-107">Yhteyden muodostaminen Microsoft 365 ja PowerShellin avulla</span><span class="sxs-lookup"><span data-stu-id="386a8-107">How to connect to Microsoft 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="386a8-108">Lisä tietoja PowerShell MsolUser-komennoista</span><span class="sxs-lookup"><span data-stu-id="386a8-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
