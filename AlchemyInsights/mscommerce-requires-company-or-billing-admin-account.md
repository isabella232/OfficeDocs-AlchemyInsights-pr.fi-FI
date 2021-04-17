---
title: Yhteyden muodostaminen MSCommerce-moduuliin
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
- "9001212"
- "3529"
ms.openlocfilehash: 8e6819f6d6ff37baab4bdd49cb5a87c32490f841
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51829733"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a><span data-ttu-id="6fb4c-102">MSCommerce edellyttää yrityksen tai laskutuksen järjestelmänvalvojan tiliä</span><span class="sxs-lookup"><span data-stu-id="6fb4c-102">MSCommerce requires a Company or Billing Administrator account</span></span>

<span data-ttu-id="6fb4c-103">MSCommerce-moduuli edellyttää tiliä, jolla on yrityksen tai laskutuksen järjestelmänvalvojan oikeudet.</span><span class="sxs-lookup"><span data-stu-id="6fb4c-103">The MSCommerce module requires an account with Company or Billing Administrator privileges.</span></span> <span data-ttu-id="6fb4c-104">Jos saat seuraavan virheilmoituksen, sinun on yhdistettävä uudelleen toiseen tiliin.</span><span class="sxs-lookup"><span data-stu-id="6fb4c-104">If you are receiving the following error, you will need to reconnect with a different account.</span></span>

<span data-ttu-id="6fb4c-105">*ErrorMessage – etäpalvelin palautti virheen: (403) Kielletty. ErrorDetails – At C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*</span><span class="sxs-lookup"><span data-stu-id="6fb4c-105">*ErrorMessage - The remote server returned an error: (403) Forbidden. ErrorDetails - At C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*</span></span><br>
<span data-ttu-id="6fb4c-106">*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Epäonnistui...*</span><span class="sxs-lookup"><span data-stu-id="6fb4c-106">*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Failed to retri ...*</span></span><br>
<span data-ttu-id="6fb4c-107">\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~</span><span class="sxs-lookup"><span data-stu-id="6fb4c-107">\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~</span></span><br>
<span data-ttu-id="6fb4c-108">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo : NotSpecified: (:) [Kirjoitusvirhe], WriteErrorException*</span><span class="sxs-lookup"><span data-stu-id="6fb4c-108">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo          : NotSpecified: (:) [Write-Error], WriteErrorException*</span></span><br>
<span data-ttu-id="6fb4c-109">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId: Microsoft.PowerShell.Commands.WriteErrorException,HandleError*</span><span class="sxs-lookup"><span data-stu-id="6fb4c-109">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*</span></span>

<span data-ttu-id="6fb4c-110">Jos tililläsi ei ole yrityksen tai laskutuksen järjestelmänvalvojan oikeuksia, ota yhteyttä IT-järjestelmänvalvojaan.</span><span class="sxs-lookup"><span data-stu-id="6fb4c-110">If your account does not have Company or Billing Administrator privileges, contact your IT Admin.</span></span>
