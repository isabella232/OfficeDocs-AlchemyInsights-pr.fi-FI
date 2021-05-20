---
title: Suojauskeskuksessa ei löytynyt tilausviestiä
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544105"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="bb465-102">Suojauskeskuksessa ei löytynyt tilausviestiä</span><span class="sxs-lookup"><span data-stu-id="bb465-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="bb465-103">Jos Microsoft Defender Security Center käytön aikana saat "Tilauksia ei löytynyt" -viestin, se tarkoittaa, että Azure Active Directory (AAD), jolla käyttäjä kirjautuu portaaliin, ei ole Microsoft Defender ATP käyttöoikeutta.</span><span class="sxs-lookup"><span data-stu-id="bb465-103">If while accessing Microsoft Defender Security Center you get a "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="bb465-104">E5 Windows ja Office E5 -käyttöoikeudet ovat erillisiä käyttöoikeuksia.</span><span class="sxs-lookup"><span data-stu-id="bb465-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="bb465-105">Avaa tukitapaus, jos käyttöoikeus on ostettu, mutta sitä ei ole määritetty tähän AAD-esiintymään.</span><span class="sxs-lookup"><span data-stu-id="bb465-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="bb465-106">Sinulla on joko:</span><span class="sxs-lookup"><span data-stu-id="bb465-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="bb465-107">Mahdollinen käyttöoikeuksien valmisteluongelma.</span><span class="sxs-lookup"><span data-stu-id="bb465-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="bb465-108">Olet vahingossa valmistella käyttöoikeuden eri Microsoft AAD:lle kuin palveluun todentamiseen käytetty käyttöoikeus.</span><span class="sxs-lookup"><span data-stu-id="bb465-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>