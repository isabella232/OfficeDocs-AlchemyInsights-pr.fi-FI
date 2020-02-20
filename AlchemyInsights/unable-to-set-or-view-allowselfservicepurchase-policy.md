---
title: AllowSelfServicePurchase-käytäntöä ei voi määrittää tai tarkastella
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158558"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="52cd3-102">AllowSelfServicePurchase-käytäntöä ei voi määrittää tai tarkastella</span><span class="sxs-lookup"><span data-stu-id="52cd3-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="52cd3-103">Kun yrität määrittää tai tarkastella AllowSelfServicePurchase-käytäntöä, näyttöön tulee seuraava virhesanoma:</span><span class="sxs-lookup"><span data-stu-id="52cd3-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="52cd3-104">*HandleError : Tuotekäytännön noutaminen PolicyId'AllowSelfServicePurchase-, ErrorMessage - Pohjana oleva yhteys katkaistiin: Lähetyksen yhteydessä tapahtui odottamaton virhe.*</span><span class="sxs-lookup"><span data-stu-id="52cd3-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="52cd3-105">Tämä saattaa johtua TLS (Transport Layer Security) -järjestelmän vanhemmasta versiosta.</span><span class="sxs-lookup"><span data-stu-id="52cd3-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="52cd3-106">Jos haluat yhdistää MSCommerce-palvelun, sinun on käytettävä TLS 1.2:ta tai uudempaa.</span><span class="sxs-lookup"><span data-stu-id="52cd3-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="52cd3-107">Ota TLS-protokolla käyttöön tai määritä sen arvoksi 1.2, tarkista ja yritä uudelleen seuraavasti.</span><span class="sxs-lookup"><span data-stu-id="52cd3-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="52cd3-108">Määritä TLS-protokollaversioksi versio\) 1.2 kirjoittamalla PowerShell-komentokehotteeseen (PS C: seuraava komento:</span><span class="sxs-lookup"><span data-stu-id="52cd3-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="52cd3-109">Tarkista käytössä olevat TLS-protokollat seuraavalla komennolla:</span><span class="sxs-lookup"><span data-stu-id="52cd3-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="52cd3-110">Yritä Get- tai Update-komentoja uudelleen tarpeen mukaan.</span><span class="sxs-lookup"><span data-stu-id="52cd3-110">Retry the Get or Update commands as needed.</span></span>

