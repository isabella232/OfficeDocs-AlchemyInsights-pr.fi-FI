---
title: Allowseldo-osto käytäntöä ei voi asettaa tai tarkastella
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
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735196"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="c7dc6-102">Allowseldo-osto käytäntöä ei voi asettaa tai tarkastella</span><span class="sxs-lookup"><span data-stu-id="c7dc6-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="c7dc6-103">Näyttöön tulee seuraava virhe sanoma, kun yrität asettaa tai tarkastella Allowselksservicepurchase-käytäntöä:</span><span class="sxs-lookup"><span data-stu-id="c7dc6-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="c7dc6-104">*HandleError: ei voitu noutaa tuote käytäntöä ja PolicyId ' AllowSelfServicePurchase ', ErrorMessage-perustana oleva yhteys suljettiin: Odottamaton virhe lähetettäessä.*</span><span class="sxs-lookup"><span data-stu-id="c7dc6-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="c7dc6-105">Tämä voi johtua siitä, että TLS on vanha versio.</span><span class="sxs-lookup"><span data-stu-id="c7dc6-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="c7dc6-106">Jos haluat yhdistää MSCommerce-palvelun, sinun on käytettävä TLS 1,2 tai uudempaa.</span><span class="sxs-lookup"><span data-stu-id="c7dc6-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="c7dc6-107">Kokeile seuraavia vaiheita, jos haluat ottaa TLS-protokollan käyttöön tai asettaa sen 1,2, vahvistaa ja yrittää uudelleen.</span><span class="sxs-lookup"><span data-stu-id="c7dc6-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="c7dc6-108">PowerShell-komento kehotteessa (PS C: \) Kirjoita seuraava komento, jos haluat määrittää TLS-protokollan versioon 1,2:</span><span class="sxs-lookup"><span data-stu-id="c7dc6-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="c7dc6-109">Tarkista käytössä oleva TLS-protokolla ja seuraava komento:</span><span class="sxs-lookup"><span data-stu-id="c7dc6-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="c7dc6-110">Yritä hakea tai päivittää komentoja tarvittaessa uudelleen.</span><span class="sxs-lookup"><span data-stu-id="c7dc6-110">Retry the Get or Update commands as needed.</span></span>

