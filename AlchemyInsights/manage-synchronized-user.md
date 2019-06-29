---
title: Synkronoitujen käyttäjien hallinta
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
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380502"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="5c593-102">Määritä ensisijainen sähköpostiosoite tai muuta käyttäjän määritteitä ei voi</span><span class="sxs-lookup"><span data-stu-id="5c593-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="5c593-103">Jos hakemiston synkronointi on käytössä ympäristössäsi käyttäjällä tai objektilla joitakin määritteitä ei voi muuttaa hallintakeskukseen.</span><span class="sxs-lookup"><span data-stu-id="5c593-103">If directory synchronization is enabled for your environment some user or object attributes cannot be changed using the Admin Center.</span></span>
<span data-ttu-id="5c593-104">Voit hallita täysin synkronoitujen käyttäjien ja niiden määritteet, käytä paikallisen active Directoryn käyttäjien ja ryhmien hallintakonsoli (adsiedit.msc-tiedostoa).</span><span class="sxs-lookup"><span data-stu-id="5c593-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="5c593-105">Vaihtoehtoisesti voit muuttaa yksittäisten käyttäjien tai synkronoitu käyttäjät käyttävät näitä yleisiä esimerkkejä kuten näkyy powershell määritteet:</span><span class="sxs-lookup"><span data-stu-id="5c593-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="5c593-106">Set-MsolUser - UserPrincipalName-user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="5c593-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="5c593-107">Set-MsolUser - UserPrincipalName ”user@yourdomain.onmicrosoft.com” - DisplayName ”Test käyttäjä” - Sukunimi ”käyttäjä”-osasto ”Manager”-”HR-osasto</span><span class="sxs-lookup"><span data-stu-id="5c593-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="5c593-108">UserPrincipalName - Poista-MsolUser-user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="5c593-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>