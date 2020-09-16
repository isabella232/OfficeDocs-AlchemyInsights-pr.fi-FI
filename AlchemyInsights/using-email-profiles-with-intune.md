---
title: Sähkö posti profiilien käyttäminen Intunella
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653285"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="395ea-102">Sähkö posti profiilien käyttäminen Intunella</span><span class="sxs-lookup"><span data-stu-id="395ea-102">Using email profiles with Intune</span></span>

<span data-ttu-id="395ea-103">Intunella voi luoda ja ottaa käyttöön Sähkö posti profiileja, jotka koskevat alkuperäistä (sisäänrakennettua) sähkö posti ohjelmaa useilla laite alustoilla.</span><span class="sxs-lookup"><span data-stu-id="395ea-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="395ea-104">Lisä tietoja Sähkö posti profiileihin liittyvistä rajoituksista, kuten olemassa olevien profiilien käytöstä ja Sähkö posti profiilien poistamisesta, on Ohje aiheessa [Sähkö posti asetusten lisääminen laitteisiin Intune-toiminnon avulla](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="395ea-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="395ea-105">Lisä tietoja Sähkö posti profiilien luomisesta kullekin laite alustalle on kohdassa:</span><span class="sxs-lookup"><span data-stu-id="395ea-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="395ea-106">Android-laitteen asetukset sähkö postin, todennuksen ja synkronoinnin määrittämiseen Intunella</span><span class="sxs-lookup"><span data-stu-id="395ea-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="395ea-107">Sähkö posti asetusten lisääminen iOS-ja iPadOS-laitteille Microsoft Intunella</span><span class="sxs-lookup"><span data-stu-id="395ea-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="395ea-108">Sähkö posti profiilin asetukset Microsoft Intunella Windows Phone 8,1-laitteita varten</span><span class="sxs-lookup"><span data-stu-id="395ea-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="395ea-109">Windows 10: n laitteiden Sähkö posti profiilin asetukset Microsoft Intunella</span><span class="sxs-lookup"><span data-stu-id="395ea-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="395ea-110">**Yleinen synkronointi ongelma**</span><span class="sxs-lookup"><span data-stu-id="395ea-110">**Common syncing issue**</span></span>

<span data-ttu-id="395ea-111">**Android-Sähkö posti profiilissa oleva KNOX estää käyttäjä kontakteja, kalenteria ja tehtäviä synkronoimasta käyttäjän laitteisiin.**</span><span class="sxs-lookup"><span data-stu-id="395ea-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="395ea-112">Android-KNOX-Sähkö posti profiilissa oleva KNOX tarjoaa järjestelmänvalvojalle mahdollisuuden määrittää, mitkä sisältö tyypit synkronoidaan laitteeseen, määrittämällä kukin käyttöön.</span><span class="sxs-lookup"><span data-stu-id="395ea-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="395ea-113">Jos minkä tahansa sisältö tyypin asetusta **ei ole määritetty** (oletus arvo), kyseistä sisältö tyyppiä ei synkronoida automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="395ea-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="395ea-114">Käyttäjä voi ottaa käyttöön sisältö tyypin, jonka he haluavat suoraan laitteeseen manuaalisesti, mutta tämä kokoonpano korvataan Intune-asetuksella ja sisältö tyypin synkronointi pysähtyy.</span><span class="sxs-lookup"><span data-stu-id="395ea-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

