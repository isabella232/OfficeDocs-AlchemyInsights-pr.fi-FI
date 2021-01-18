---
title: Virtuaalinen määritys AAD-toimialueen palvelujen kanssa
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885201"
---
# <a name="virtual-configuration-with-aad-domain-services"></a><span data-ttu-id="f0b9f-102">Virtuaalinen määritys AAD-toimialueen palvelujen kanssa</span><span class="sxs-lookup"><span data-stu-id="f0b9f-102">Virtual configuration with AAD domain services</span></span>

<span data-ttu-id="f0b9f-103">Virtuaalimäärityksessä AAD-toimialueen palveluissa on seuraavat vaiheet:</span><span class="sxs-lookup"><span data-stu-id="f0b9f-103">Virtual configuration with AAD domain services involves the following steps:</span></span> 

1. <span data-ttu-id="f0b9f-104">Toimialueen kuntotarkistuksen tarkistaminen Azure-portaalissa https://aka.ms/aadds-health</span><span class="sxs-lookup"><span data-stu-id="f0b9f-104">Checking your domain’s health on the Azure portal https://aka.ms/aadds-health</span></span>
2. <span data-ttu-id="f0b9f-105">NSG:n tarkistaminen sääntöjä, jotka estävät portit, jotka tarvitaan portaalin Azure AD -toimialueen palveluissa synkronoinnissa https://aka.ms/aadds-networking</span><span class="sxs-lookup"><span data-stu-id="f0b9f-105">Checking your NSG for rules that block ports needed to synchronize in Azure AD Domain Services on the portal https://aka.ms/aadds-networking</span></span>
3. <span data-ttu-id="f0b9f-106">Sen varmistaminen, että virtuaalinen verkostosi otetaan käyttöön samalla Azure-alueella kuin Azure AD -toimialueen palveluiden hallinnoimaa toimialuetta.</span><span class="sxs-lookup"><span data-stu-id="f0b9f-106">Ensuring that your virtual network is deployed in the same Azure Region as your Azure AD Domain Services-managed domain.</span></span>
4. <span data-ttu-id="f0b9f-107">Sen varmistaminen, että sinulla ei ole olemassa toimialuetta, jolla on sama toimialuenimi käytettävissä virtuaaliverkossa.</span><span class="sxs-lookup"><span data-stu-id="f0b9f-107">Ensuring you don’t have an existent domain with the same domain name available on the virtual network.</span></span>

<span data-ttu-id="f0b9f-108">Lisätietoja AAD-toimialueen palveluja tukevan Azure Virtual Networkin suunnittelusta on virtual [network consideration -palvelussa.](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations)</span><span class="sxs-lookup"><span data-stu-id="f0b9f-108">For more details on design consideration on Azure Virtual Network to support AAD domain services, see [Virtual Network Consideration](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span></span>

