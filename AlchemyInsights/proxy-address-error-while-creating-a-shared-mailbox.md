---
title: Välityspalvelimen osoitevirhe jaetun postilaatikon luonnin aikana
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568287"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a><span data-ttu-id="0304d-102">Välityspalvelimen osoitevirhe luotaessa postilaatikkoa tai muuta sähköpostia käyttävää objektia</span><span class="sxs-lookup"><span data-stu-id="0304d-102">Proxy address error while creating a mailbox or other email enabled object</span></span>

<span data-ttu-id="0304d-103">Jos yritit luoda sähköpostia käyttävän objektin (postilaatikko, jaettu postilaatikko jne.) ja sait virhesanoman "Välityspalvelimen osoite "SMTP:alias@domain.com" on jo käytössä...", valitsemasi sähköpostiosoite on jo toisen organisaation sähköpostia käyttävän objektin käytössä.</span><span class="sxs-lookup"><span data-stu-id="0304d-103">If you tried to create an email-enabled object (mailbox, shared mailbox etc.) and received the error "The proxy address "SMTP:alias@domain.com" is already being used…", the email address you chose is already taken by another email-enabled object in your organization.</span></span>
  
<span data-ttu-id="0304d-104">Sinun on etsittava käyttäjä, ryhmä, jaettu postilaatikko tai yleinen kansio, jossa tämä sähköpostiosoite on, ja poistettava se tai muutettava sen sähköpostiosoitetta.</span><span class="sxs-lookup"><span data-stu-id="0304d-104">You need to find the user, group, shared mailbox or public folder that has this email address and delete it or change its email address.</span></span> <span data-ttu-id="0304d-105">Sen jälkeen voit luoda uuden sähköpostia käyttävän objektin, jossa on vapaita sähköpostiosoitteita.</span><span class="sxs-lookup"><span data-stu-id="0304d-105">Then you can create a new email-enabled object with the freed email address.</span></span> <span data-ttu-id="0304d-106">Etsi se aloitussivun Haku-haun avulla.</span><span class="sxs-lookup"><span data-stu-id="0304d-106">Use Search on the Home page to find it.</span></span> <span data-ttu-id="0304d-107">Voit etsiä sitä myös seuraavan Exchange Online PowerShell -komennon avulla:</span><span class="sxs-lookup"><span data-stu-id="0304d-107">You can also use the following Exchange Online PowerShell command to search for it:</span></span>

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
<span data-ttu-id="0304d-108">Jos et halua poistaa olemassa olevaa sähköpostiosoitetta, valitse uusi sähköpostiosoite luomallesi uudelle objektille.</span><span class="sxs-lookup"><span data-stu-id="0304d-108">If you don't want to delete the existing email address, choose a new email address for the new object you are creating.</span></span>
  