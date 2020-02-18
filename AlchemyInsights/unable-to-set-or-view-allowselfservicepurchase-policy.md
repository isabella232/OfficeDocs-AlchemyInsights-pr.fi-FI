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
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091694"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="3a81f-102">AllowSelfServicePurchase-käytäntöä ei voi määrittää tai tarkastella</span><span class="sxs-lookup"><span data-stu-id="3a81f-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="3a81f-103">Kun yrität määrittää tai tarkastella AllowSelfServicePurchase-käytäntöä, näyttöön tulee seuraava virhesanoma:</span><span class="sxs-lookup"><span data-stu-id="3a81f-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="3a81f-104">*HandleError : Tuotekäytännön noutaminen PolicyId'AllowSelfServicePurchase-, ErrorMessage - Pohjana oleva yhteys katkaistiin: Lähetyksen yhteydessä tapahtui odottamaton virhe.*</span><span class="sxs-lookup"><span data-stu-id="3a81f-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="3a81f-105">Tämä saattaa johtua TLS (Transport Layer Security) -järjestelmän vanhemmasta versiosta.</span><span class="sxs-lookup"><span data-stu-id="3a81f-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="3a81f-106">Jos haluat yhdistää MSCommerce-palvelun, sinun on käytettävä TLS 1.2:ta tai uudempaa.</span><span class="sxs-lookup"><span data-stu-id="3a81f-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="3a81f-107">Ota TLS-protokolla käyttöön tai määritä sen arvoksi 1.2, tarkista ja yritä uudelleen seuraavasti.</span><span class="sxs-lookup"><span data-stu-id="3a81f-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="3a81f-108">Määritä TLS-protokollaversioksi versio\) 1.2 kirjoittamalla PowerShell-komentokehotteeseen (PS C: seuraava komento:</span><span class="sxs-lookup"><span data-stu-id="3a81f-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    <span data-ttu-id="3a81f-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span><span class="sxs-lookup"><span data-stu-id="3a81f-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span></span>

2. <span data-ttu-id="3a81f-110">Tarkista käytössä olevat TLS-protokollat seuraavalla komennolla:</span><span class="sxs-lookup"><span data-stu-id="3a81f-110">Verify the TLS protocol(s) in use, with the following command:</span></span>

    <span data-ttu-id="3a81f-111">\[Net.ServicePointManager]::Suojausprotokolla</span><span class="sxs-lookup"><span data-stu-id="3a81f-111">\[Net.ServicePointManager]::SecurityProtocol</span></span> 

3. <span data-ttu-id="3a81f-112">Yritä Get- tai Update-komentoja uudelleen tarpeen mukaan.</span><span class="sxs-lookup"><span data-stu-id="3a81f-112">Retry the Get or Update commands as needed.</span></span>

