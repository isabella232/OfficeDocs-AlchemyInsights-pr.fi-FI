---
title: Microsoft Edgeen kirjautuminen automaattisesti
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398726"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="57c64-102">Microsoft Edgeen kirjautuminen automaattisesti</span><span class="sxs-lookup"><span data-stu-id="57c64-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="57c64-103">Microsoft Edge käyttää käyttöjärjestelmän oletustiliä käyttäjän automaattinen kirjautuminen käyttäjän laitteen määritysten mukaan.</span><span class="sxs-lookup"><span data-stu-id="57c64-103">Microsoft Edge uses the OS default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="57c64-104">Kunkin laitekokoonpanon ja sen riippuvaisen käyttäjän kirjautumisprosessin skenaariot on kuvattu alla:</span><span class="sxs-lookup"><span data-stu-id="57c64-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

- <span data-ttu-id="57c64-105">**Laite on yhdistelmäympäristö/AAD-J:** Tämä asetus on käytettävissä Windows 10:ssä, windowsissa ja sitä vastaavissa palvelinversioissa.</span><span class="sxs-lookup"><span data-stu-id="57c64-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="57c64-106">Käyttäjät kirjautuvat automaattisesti Azure Active Directory (AD) -tileinsä avulla.</span><span class="sxs-lookup"><span data-stu-id="57c64-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
- <span data-ttu-id="57c64-107">**Laite on liitetty toimialueeseen:** Tämä asetus on käytettävissä Windows 10:ssä, Windowsissa ja sitä vastaavissa palvelinversioissa.</span><span class="sxs-lookup"><span data-stu-id="57c64-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="57c64-108">Käyttäjät, joilla on toimialuetili, eivät oletusarvoisesti kirjaudu sisään automaattisesti. jos haluat ottaa automaattisen kirjautumisen käyttöön, käytä **ConfigureOnPremisesAccountAutoSignIn-käytäntöä.**</span><span class="sxs-lookup"><span data-stu-id="57c64-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="57c64-109">Jos haluat ottaa automaattisen kirjautumisen käyttöön Azure AD -tilejä käyttäjillä, harkitse yhdistelmäympäristön liittämistä heidän laitteisiinsa.</span><span class="sxs-lookup"><span data-stu-id="57c64-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
- <span data-ttu-id="57c64-110">**Käyttöjärjestelmän oletustili** on Microsoft-tili: Tämä asetus on käytettävissä Windows 10 RS3:ssa (versio 1709, koontiversio 10.0.16299) ja myommissa versioissa.</span><span class="sxs-lookup"><span data-stu-id="57c64-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="57c64-111">Skenaariota ei todennäköisesti ilmene yrityslaitteilla.</span><span class="sxs-lookup"><span data-stu-id="57c64-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="57c64-112">Jos käyttöjärjestelmän oletustili on Microsoft-tili, Microsoft Edge kirjautuu automaattisesti sisään käyttäjälle Microsoft-tilillä.</span><span class="sxs-lookup"><span data-stu-id="57c64-112">However, if the OS default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
