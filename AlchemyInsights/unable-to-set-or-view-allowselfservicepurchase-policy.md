---
title: AllowSelfServicePurchase-käytännön joukon tai tarkasteleminen ei onnistu
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
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826088"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="d3178-102">AllowSelfServicePurchase-käytännön joukon tai tarkasteleminen ei onnistu</span><span class="sxs-lookup"><span data-stu-id="d3178-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="d3178-103">Kun yrität määrittää tai tarkastella AllowSelfServicePurchase-käytäntöä, näyttöön tulee seuraava virhesanoma:</span><span class="sxs-lookup"><span data-stu-id="d3178-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="d3178-104">*HandleError: Tuotekäytännön noutaminen epäonnistui, kun PolicyId on AllowSelfServicePurchase, ErrorMessage - Pohjana oleva yhteys suljettiin: Lähetystä käsiteltäessä tapahtui odottamaton virhe.*</span><span class="sxs-lookup"><span data-stu-id="d3178-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="d3178-105">Tämä voi johtua TLS (Transport Layer Security) -suojausversion vanhemman version vuoksi.</span><span class="sxs-lookup"><span data-stu-id="d3178-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="d3178-106">Jos haluat yhdistää MSCommerce-palvelun, sinun on käytettävä TLS 1.2:ta tai sitä uudempia.</span><span class="sxs-lookup"><span data-stu-id="d3178-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="d3178-107">Seuraavien vaiheiden avulla voit ottaa TLS-protokollan käyttöön tai määrittää sen arvoksi 1.2, tarkistaa ja yrittää uudelleen.</span><span class="sxs-lookup"><span data-stu-id="d3178-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="d3178-108">Määritä TLS-protokolla versioksi 1.2 kirjoittamalla PowerShell-komentokehotteeseen (PS C: määritä \) TLS-protokolla versioon 1.2:</span><span class="sxs-lookup"><span data-stu-id="d3178-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="d3178-109">Varmista, että TLS-protokollat ovat käytössä, seuraavalla komennolla:</span><span class="sxs-lookup"><span data-stu-id="d3178-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="d3178-110">Yritä tarvittaessa Hae- tai Päivitä-komentoja uudelleen.</span><span class="sxs-lookup"><span data-stu-id="d3178-110">Retry the Get or Update commands as needed.</span></span>

