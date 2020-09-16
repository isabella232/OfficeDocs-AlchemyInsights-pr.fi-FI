---
title: Intune-käytäntöjen ja-profiilien luominen
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1064"
- "6700005"
ms.openlocfilehash: 9026beac824ebc3849241dbb534c27b00ef1d0eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47746756"
---
# <a name="creating-intune-policy-and-profiles"></a><span data-ttu-id="b9b27-102">Intune-käytäntöjen ja-profiilien luominen</span><span class="sxs-lookup"><span data-stu-id="b9b27-102">Creating Intune policy and profiles</span></span>

<span data-ttu-id="b9b27-103">Intunella voit luoda käytäntöjä ja profiileja, jotka tekevät erilaisia asioita.</span><span class="sxs-lookup"><span data-stu-id="b9b27-103">In Intune, you can create policies and profiles that do different things.</span></span>

- <span data-ttu-id="b9b27-104">**Rekisteröinti profiilit**: Määritä laitteet alusta alkaen, ota käyttöön käyttäjien affiniteetti, käytä monimenetelmäistä todennusta ja paljon muuta.</span><span class="sxs-lookup"><span data-stu-id="b9b27-104">**Enrollment profiles**: Preconfigure your devices by platform, enable user affinity, use multi-factor authentication, and more.</span></span>

  <span data-ttu-id="b9b27-105">[Mikä on laite rekisteröinti ja miten](https://docs.microsoft.com/intune/device-enrollment)luoda rekisteröinti profiileja [Android](https://docs.microsoft.com/intune/android-enroll)-, [iOS](https://docs.microsoft.com/intune/ios-enroll)-, [MacOS](https://docs.microsoft.com/intune/macos-enroll)-ja [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) -laitteille ovat hyviä resursseja.</span><span class="sxs-lookup"><span data-stu-id="b9b27-105">[What is device enrollment](https://docs.microsoft.com/intune/device-enrollment), and create enrollment profiles for [Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll), and [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) are good resources.</span></span>

- <span data-ttu-id="b9b27-106">**Yhteensopivuus käytännöt**: Määritä säännöt ja asetukset, joita laitteiden on noudatettava.</span><span class="sxs-lookup"><span data-stu-id="b9b27-106">**Compliance policies**: Define the rules and settings that devices must follow to be compliant.</span></span> <span data-ttu-id="b9b27-107">Yhteensopivuus käytäntöjen avulla voit myös valvoa laitteita ja ilmoittaa käyttäjille vaatimustenmukaisuudesta.</span><span class="sxs-lookup"><span data-stu-id="b9b27-107">You can also use compliance policies to monitor devices, and notify users of non-compliance.</span></span>

  <span data-ttu-id="b9b27-108">Aloita [laitteiden yhteensopivuus käytännöt](https://docs.microsoft.com/intune/device-compliance-get-started).</span><span class="sxs-lookup"><span data-stu-id="b9b27-108">Get started with [device compliance policies](https://docs.microsoft.com/intune/device-compliance-get-started).</span></span>
- <span data-ttu-id="b9b27-109">**Ehdollisen käytön käytännöt**: auttaa turvaamaan organisaation resursseja syöttämiesi ehtojen mukaan.</span><span class="sxs-lookup"><span data-stu-id="b9b27-109">**Conditional access policies**: Help secure organizational resources, depending on conditions that you enter.</span></span> <span data-ttu-id="b9b27-110">Jos kyseessä on esimerkiksi laite, joka ei ole yhteensopiva, käytä ehdollista käyttö oikeutta sähkö postin ja SharePointin käytön rajoittamiseen.</span><span class="sxs-lookup"><span data-stu-id="b9b27-110">For example, for devices that aren't compliant, use conditional access to restrict access to email and SharePoint.</span></span>

  <span data-ttu-id="b9b27-111">[Mikä on ehdollinen käyttö oikeus](https://docs.microsoft.com/intune/conditional-access) ja [yleisimmät ehdollisen käytön tavat](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) , ovat hyviä resursseja, joiden avulla pääset alkuun.</span><span class="sxs-lookup"><span data-stu-id="b9b27-111">[What is conditional access](https://docs.microsoft.com/intune/conditional-access) and [common ways to use conditional access](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) are good resources to get started.</span></span>

- <span data-ttu-id="b9b27-112">**Määritys profiilit**: Hallitse laitteiden ominaisuuksia ja asetuksia, kuten sähkö posti asetuksia, lisää WiFi-verkko, käytä valmiita malleja, Hallitse iOS-ja MacOS-laite ominaisuuksia ja paljon muuta.</span><span class="sxs-lookup"><span data-stu-id="b9b27-112">**Configuration profiles**: Manage features and settings on devices, including email settings, add a WiFi network, use built-in templates, control iOS and macOS device features, and more.</span></span>

  <span data-ttu-id="b9b27-113">Aloita [laitteen määritys profiileilla](https://docs.microsoft.com/intune/device-profiles).</span><span class="sxs-lookup"><span data-stu-id="b9b27-113">Get started at [device configuration profiles](https://docs.microsoft.com/intune/device-profiles).</span></span>

<span data-ttu-id="b9b27-114">Hyödyllisiä linkkejä:</span><span class="sxs-lookup"><span data-stu-id="b9b27-114">Helpful links:</span></span>

- [<span data-ttu-id="b9b27-115">Yleisiä kysymyksiä, ongelmia ja päätös lauselmia laite käytäntöjen ja-profiilien avulla Intunella</span><span class="sxs-lookup"><span data-stu-id="b9b27-115">Common questions, issues, and resolutions with device policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/device-profile-troubleshoot)

- [<span data-ttu-id="b9b27-116">Käytäntöjen ja profiilien vian määritys Intune-sovelluksessa</span><span class="sxs-lookup"><span data-stu-id="b9b27-116">Troubleshoot policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
