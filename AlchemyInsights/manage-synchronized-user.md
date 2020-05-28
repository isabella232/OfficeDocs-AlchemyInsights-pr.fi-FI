---
title: Synkronoidun käyttäjän hallinta
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 84e337a7224fdd3c3ab7ad0f61240692fe007d5a
ms.sourcegitcommit: 82af227ac6d075e748e27c4ce6bdcf56628559cb
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/28/2020
ms.locfileid: "44407347"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="e0ac0-102">Ensisijaista sähköpostiosoitetta ei voi määrittää, käyttäjämääritteitä ei voi määrittää tai synkronoitua käyttäjää ei voi poistaa tai poistaa</span><span class="sxs-lookup"><span data-stu-id="e0ac0-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="e0ac0-103">Jos hakemistosynkronointi on käytössä ympäristössäsi, joitakin käyttäjän tai objektin määritteitä ei voi muuttaa Microsoft 365 -hallintakeskuksen avulla.</span><span class="sxs-lookup"><span data-stu-id="e0ac0-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="e0ac0-104">Jos haluat hallita synkronoituja käyttäjiä ja kaikkia heidän määritteitään täysin, käytä paikallisia active directory -käyttäjiä ja ryhmien hallintakonsolia (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="e0ac0-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="e0ac0-105">Vaihtoehtoisesti voit muuttaa synkronoitujen käyttäjien yksittäisiä käyttäjiä tai määritteitä PowerShellin avulla, kuten seuraavissa yleisissä esimerkeissä:</span><span class="sxs-lookup"><span data-stu-id="e0ac0-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
