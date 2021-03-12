---
title: Suojauskeskuksesta ei löytynyt tilauksia
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
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "50713602"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="49e97-102">Suojauskeskuksesta ei löytynyt tilauksia</span><span class="sxs-lookup"><span data-stu-id="49e97-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="49e97-103">Jos saat Microsoft Defender Security Centeriä käytön aikana viestin "Tilauksia ei löytynyt", se tarkoittaa, että Azure Active Directory (AAD), jolla käyttäjä kirjautuu portaaliin, ei ole Microsoft Defender ATP -käyttöoikeutta.</span><span class="sxs-lookup"><span data-stu-id="49e97-103">If while accessing Microsoft Defender Security Center you get a  "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="49e97-104">Windows E5- ja Office E5 -käyttöoikeudet ovat erillisiä käyttöoikeuksia.</span><span class="sxs-lookup"><span data-stu-id="49e97-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="49e97-105">Avaa tukitapaus, jos käyttöoikeus on ostettu, mutta sitä ei ole määritetty tähän AAD-esiintymään.</span><span class="sxs-lookup"><span data-stu-id="49e97-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="49e97-106">Sinulla on jompikumpi seuraavista:</span><span class="sxs-lookup"><span data-stu-id="49e97-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="49e97-107">Mahdollinen käyttöoikeuden valmisteluongelma.</span><span class="sxs-lookup"><span data-stu-id="49e97-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="49e97-108">Olet vahingossa valmistella käyttöoikeuden eri Microsoft AAD:lle kuin palveluun todentamisessa käytetty käyttöoikeus.</span><span class="sxs-lookup"><span data-stu-id="49e97-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>