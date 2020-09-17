---
title: Synkronoidun käyttäjän hallinta
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
- "9000609"
- "2444"
ms.openlocfilehash: 53c188f6c6ab93bcc6f87d95717dc0d24d492bb7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47777674"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="3f481-102">Ei voi määrittää ensisijaisia Sähkö posti osoitteita, muuttaa käyttäjän määritteitä tai poistaa tai poistaa synkronoitua käyttäjää.</span><span class="sxs-lookup"><span data-stu-id="3f481-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="3f481-103">Jos ympäristössäsi on käytössä hakemisto synkronointi, joitakin käyttäjä-tai objekti määritteitä ei voi muuttaa Microsoft 365-hallinta keskuksen avulla.</span><span class="sxs-lookup"><span data-stu-id="3f481-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="3f481-104">Jos haluat hallita synkronoituja käyttäjiä ja niiden määritteitä täysin, käytä paikallisia Active Directory-käyttäjien ja-ryhmien hallinta konsolia (ADSIEdit. msc).</span><span class="sxs-lookup"><span data-stu-id="3f481-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="3f481-105">Voit vaihtoehtoisesti muuttaa PowerShell-toiminnon käyttäjiä tai määritteitä, kuten seuraavia yleisiä esimerkkejä:</span><span class="sxs-lookup"><span data-stu-id="3f481-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
