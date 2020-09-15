---
title: Yhteyden muodostaminen MSCommerce-moduuliin
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
- "9001212"
- "3529"
ms.openlocfilehash: 15dc7038426a8d436c236a91aa0f3462f6a3e366
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702612"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a><span data-ttu-id="da470-102">MSCommerce edellyttää yrityksen tai laskutuksen järjestelmänvalvojatiliä</span><span class="sxs-lookup"><span data-stu-id="da470-102">MSCommerce requires a Company or Billing Administrator account</span></span>

<span data-ttu-id="da470-103">MSCommerce-moduuli vaatii tilin, jossa on yrityksen tai laskutuksen järjestelmänvalvojan oikeudet.</span><span class="sxs-lookup"><span data-stu-id="da470-103">The MSCommerce module requires an account with Company or Billing Administrator privileges.</span></span> <span data-ttu-id="da470-104">Jos saat seuraavan virhe ilmoituksen, sinun on muodostettava yhteys uudelleen toisella tilillä.</span><span class="sxs-lookup"><span data-stu-id="da470-104">If you are receiving the following error, you will need to reconnect with a different account.</span></span>

<span data-ttu-id="da470-105">*Errorimessage-Etäpalvelin palautti virheen: (403) kielletty. Virheen tiedot-at C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char: 5*</span><span class="sxs-lookup"><span data-stu-id="da470-105">*ErrorMessage - The remote server returned an error: (403) Forbidden. ErrorDetails - At C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*</span></span><br>
<span data-ttu-id="da470-106">*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError-Errorecontext $ _-Custeerroremessage "Failed to retri...*</span><span class="sxs-lookup"><span data-stu-id="da470-106">*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Failed to retri ...*</span></span><br>
<span data-ttu-id="da470-107">\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~</span><span class="sxs-lookup"><span data-stu-id="da470-107">\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~</span></span><br>
<span data-ttu-id="da470-108">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ Luokan tiedot: Notmääritetty: (:) [Write-Error], Writelerroxception*</span><span class="sxs-lookup"><span data-stu-id="da470-108">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo          : NotSpecified: (:) [Write-Error], WriteErrorException*</span></span><br>
<span data-ttu-id="da470-109">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId: Microsoft. PowerShell. commands. Writterrorception, HandleError*</span><span class="sxs-lookup"><span data-stu-id="da470-109">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*</span></span>

<span data-ttu-id="da470-110">Jos tililläsi ei ole yrityksen tai laskutuksen järjestelmänvalvojan oikeuksia, ota yhteyttä IT-järjestelmänvalvojaan.</span><span class="sxs-lookup"><span data-stu-id="da470-110">If your account does not have Company or Billing Administrator privileges, contact your IT Admin.</span></span>
