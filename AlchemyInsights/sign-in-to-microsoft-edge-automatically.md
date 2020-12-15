---
title: Kirjautuminen Microsoft Edgeen automaattisesti
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
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677236"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="29a14-102">Kirjautuminen Microsoft Edgeen automaattisesti</span><span class="sxs-lookup"><span data-stu-id="29a14-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="29a14-103">Microsoft Edge käyttää käyttö järjestelmän oletus tiliä kirjautuessaan automaattisesti käyttäjän laitteeseen sen mukaan, miten käyttäjän laite on määritetty.</span><span class="sxs-lookup"><span data-stu-id="29a14-103">Microsoft Edge uses the OS's default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="29a14-104">Seuraavassa kuvataan kunkin laite tyypin ja sen riippuvaisen käyttäjän kirjautumisprosessin skenaariot:</span><span class="sxs-lookup"><span data-stu-id="29a14-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

1. <span data-ttu-id="29a14-105">**Laite on yhdistelmä/AAD-J**: Tämä vaihto ehto on käytettävissä Windows 10-, alatason Windows-ja sitä vastaavissa palvelin versioissa.</span><span class="sxs-lookup"><span data-stu-id="29a14-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="29a14-106">Käyttäjät kirjataan automaattisesti sisään Azure Active Directory (AD)-tileihinsä.</span><span class="sxs-lookup"><span data-stu-id="29a14-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
2. <span data-ttu-id="29a14-107">**Laite on liitetty toimi alueeseen**: Tämä asetus on käytettävissä Windows 10-, alatason Windows-ja sitä vastaavissa palvelin versioissa.</span><span class="sxs-lookup"><span data-stu-id="29a14-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="29a14-108">Oletusarvoisesti käyttäjät, joilla on toimi alue tiliä, eivät ole kirjautuneet sisään automaattisesti. Jos haluat ottaa automaattisen kirjautumisen käyttöön, käytä **Configureonenpremisesaccountautosigni** -käytäntöä.</span><span class="sxs-lookup"><span data-stu-id="29a14-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="29a14-109">Jos haluat ottaa käyttöön automaattisen kirjautumisen käyttäjille, joilla on Azure AD-tilisi, harkitse hybridi-liittymistään laitteisiinsa.</span><span class="sxs-lookup"><span data-stu-id="29a14-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
3. <span data-ttu-id="29a14-110">**Käyttö järjestelmän oletus tili on Microsoft-tili**: Tämä vaihto ehto on käytettävissä Windows 10 RS3 (version 1709, koonti versio 10.0.16299) ja uudemmissa versioissa.</span><span class="sxs-lookup"><span data-stu-id="29a14-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="29a14-111">Skenaario ei todennäköisesti toteudu yritys laitteissa.</span><span class="sxs-lookup"><span data-stu-id="29a14-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="29a14-112">Jos käyttö järjestelmän oletus tili on Microsoft-tili, Microsoft Edge automaattisesti kirjautuu sisään Microsoft-tilillä.</span><span class="sxs-lookup"><span data-stu-id="29a14-112">However, if the OS's default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
