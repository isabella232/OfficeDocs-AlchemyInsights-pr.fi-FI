---
title: Sähköpostiprofiilien käyttäminen Intunen kanssa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554977"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="823ed-102">Sähköpostiprofiilien käyttäminen Intunen kanssa</span><span class="sxs-lookup"><span data-stu-id="823ed-102">Using email profiles with Intune</span></span>

<span data-ttu-id="823ed-103">Intune voidaan luoda ja ottaa käyttöön sähköpostiprofiileja natiivi (sisäänrakennettu) sähköpostiohjelma useilla laitealustoilla.</span><span class="sxs-lookup"><span data-stu-id="823ed-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="823ed-104">Lisätietoja joistakin sähköpostiprofiileihin liittyvistä rajoituksista, kuten olemassa olevien profiilien käsittelytapa ja sähköpostiprofiilien poistaminen, on [ohjeaiheessa Sähköpostiasetusten lisääminen laitteisiin Intune -toiminnolla](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="823ed-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="823ed-105">Lisätietoja sähköpostiprofiilien luomisesta kullekin laitealustalle on ohjeaiheessa:</span><span class="sxs-lookup"><span data-stu-id="823ed-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="823ed-106">Android-laitteen asetukset sähköpostin, todennuksen ja synkronoinnin määrittämiseen Intuessa</span><span class="sxs-lookup"><span data-stu-id="823ed-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="823ed-107">Sähköpostiasetusten lisääminen iOS- ja iPadOS-laitteille Microsoft Intutiin</span><span class="sxs-lookup"><span data-stu-id="823ed-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="823ed-108">Microsoft Intunen sähköpostiprofiilin asetukset Windows Phone 8.1 -laitteissa</span><span class="sxs-lookup"><span data-stu-id="823ed-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="823ed-109">Sähköpostiprofiiliasetukset laitteille, joissa on Windows 10 Microsoft Intunen</span><span class="sxs-lookup"><span data-stu-id="823ed-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="823ed-110">**Yleinen synkronointiongelma**</span><span class="sxs-lookup"><span data-stu-id="823ed-110">**Common syncing issue**</span></span>

<span data-ttu-id="823ed-111">**KNOX Android-sähköpostiprofiilissa estää käyttäjän yhteystietojen, kalenterin ja tehtävien synkronoinnin käyttäjän laitteisiin.**</span><span class="sxs-lookup"><span data-stu-id="823ed-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="823ed-112">Knox Android KNOX -sähköpostiprofiilissa tarjoaa järjestelmänvalvojalle mahdollisuuden päättää, mitkä sisältötyypit synkronoidaan laitteeseen asettamalla kukin käyttöön.</span><span class="sxs-lookup"><span data-stu-id="823ed-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="823ed-113">Jos jonkin sisältötyypin asetuksena on **Ei määritetty** (oletusasetus), kyseistä sisältötyyppiä ei synkronoida automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="823ed-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="823ed-114">Käyttäjä saattaa ottaa haluamasi sisältötyypin käyttöön suoraan laitteeseen manuaalisesti, mutta Intune-käytäntöasetus korvaa kyseisen kokoonpanon ja kyseisen sisältötyypin synkronointi pysähtyy.</span><span class="sxs-lookup"><span data-stu-id="823ed-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

