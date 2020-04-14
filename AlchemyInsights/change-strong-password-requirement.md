---
title: Muuta vahva salasanavaatimus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 21f80a7cc8b00ac56acdb05add1e1bfdfac9d827
ms.sourcegitcommit: c061f1dfa6f557a9ec083dd030b73b121d9864ea
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/14/2020
ms.locfileid: "43286260"
---
# <a name="change-strong-password-requirement"></a><span data-ttu-id="4cd1c-102">Vahvan salasanavaatimuksen muuttaminen</span><span class="sxs-lookup"><span data-stu-id="4cd1c-102">Change strong password requirement</span></span>

<span data-ttu-id="4cd1c-103">Microsoft vaatii oletusarvoisesti vahvat salasanat.</span><span class="sxs-lookup"><span data-stu-id="4cd1c-103">Microsoft requires strong passwords by default.</span></span> 

<span data-ttu-id="4cd1c-104">PowerShellin avulla voit poistaa tiettyjen käyttäjien vahvat salasanat käytöstä tällä komennolla:</span><span class="sxs-lookup"><span data-stu-id="4cd1c-104">Using PowerShell, you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="4cd1c-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired $false*</span><span class="sxs-lookup"><span data-stu-id="4cd1c-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="4cd1c-106">Lisätietoja salasanakäytännöstä</span><span class="sxs-lookup"><span data-stu-id="4cd1c-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="4cd1c-107">Yhteyden muodostaminen Office 365:een PowerShellin avulla</span><span class="sxs-lookup"><span data-stu-id="4cd1c-107">How to connect to Office 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="4cd1c-108">Lisätietoja PowerShell MsolUser -komennoista</span><span class="sxs-lookup"><span data-stu-id="4cd1c-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
- [<span data-ttu-id="4cd1c-109">Yksittäisen käyttäjän salasanan määrittäminen niin, ettei se vanhene koskaan</span><span class="sxs-lookup"><span data-stu-id="4cd1c-109">Set an individual user's password to never expire</span></span>](https://docs.microsoft.com/microsoft-365/admin/add-users/set-password-to-never-expire)
