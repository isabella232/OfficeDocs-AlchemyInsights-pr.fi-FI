---
title: Vaihda vahva salasanavaatimus
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: cf5cab9a1c2dd4226997d93417dc7104347f8a6e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818465"
---
# <a name="change-strong-password-requirement"></a><span data-ttu-id="5a34e-102">Vaihda vahva salasanavaatimus</span><span class="sxs-lookup"><span data-stu-id="5a34e-102">Change strong password requirement</span></span>

<span data-ttu-id="5a34e-103">Microsoft edellyttää oletusarvoisesti vahvoja salasanoja.</span><span class="sxs-lookup"><span data-stu-id="5a34e-103">Microsoft requires strong passwords by default.</span></span>

<span data-ttu-id="5a34e-104">PowerShellin avulla voit poistaa tiettyjen käyttäjien vahvat salasanat käytöstä näillä komennoilla:</span><span class="sxs-lookup"><span data-stu-id="5a34e-104">Using PowerShell, you can disable strong passwords for specific users with these commands:</span></span>

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

<span data-ttu-id="5a34e-105">Jos haluat poistaa vahvat salasanat käytöstä käyttäjiltä, käytä:</span><span class="sxs-lookup"><span data-stu-id="5a34e-105">To disable strong passwords for all users, use:</span></span>

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [<span data-ttu-id="5a34e-106">Lisätietoja salasanakäytäntöön liittyen</span><span class="sxs-lookup"><span data-stu-id="5a34e-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="5a34e-107">Yhteyden muodostaminen Microsoft 365:seen PowerShellin avulla</span><span class="sxs-lookup"><span data-stu-id="5a34e-107">How to connect to Microsoft 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="5a34e-108">Lisätietoja PowerShellin MsolUser-komennoista</span><span class="sxs-lookup"><span data-stu-id="5a34e-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
