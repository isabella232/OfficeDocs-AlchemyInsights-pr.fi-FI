---
title: PowerShellin omatoiminen hankinta
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
- "3516"
ms.openlocfilehash: 48b5b0a1be1bc03d45a531a1093f18a3f750c37d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51797718"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="3a24c-102">PowerShellin omatoiminen hankinta</span><span class="sxs-lookup"><span data-stu-id="3a24c-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="3a24c-103">Jos haluat käyttää MSCommerce PowerShell -moduulia, sinun on asennettava se Windows 10 -laitteeseen, jossa on TLS 1.2 (edellyttää paikallisen järjestelmänvalvojan oikeuksia).</span><span class="sxs-lookup"><span data-stu-id="3a24c-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="3a24c-104">Tuo MSCommerce-moduuli ja muodosta yhteys moduuliin.</span><span class="sxs-lookup"><span data-stu-id="3a24c-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="3a24c-105">Kun sinua pyydetään kirjautumaan sisään, sinun on käytettävä yleisen tai laskutuksen järjestelmänvalvojan roolin tunnistetietoja.</span><span class="sxs-lookup"><span data-stu-id="3a24c-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="3a24c-106">Jos sinulla ei ole TLS 1.2:ta, näyttöön voi tulla seuraava virhesanoma, kun yrität saada tai päivittää käytäntöä:</span><span class="sxs-lookup"><span data-stu-id="3a24c-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="3a24c-107">*ErrorMessage -Pohjana oleva yhteys suljettiin: Lähetystä käsiteltäessä tapahtui odottamaton virhe.*</span><span class="sxs-lookup"><span data-stu-id="3a24c-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



