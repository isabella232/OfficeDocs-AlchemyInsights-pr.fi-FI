---
title: 'Www-käytön hallinta Microsoft Intunen avulla Microsoft Edge for iOS: ssä ja Androidissa'
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003846"
- "6895"
- "9006502"
- "11144"
ms.openlocfilehash: a6c6f9563933b7cf6b71c4758c29ffd94617c4be
ms.sourcegitcommit: 7a406a3d4680662e81f0056454f7e25fb2f52504
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/17/2021
ms.locfileid: "52989664"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="268c1-102">Www-käytön hallinta Microsoft Intunen avulla Microsoft Edge for iOS: ssä ja Androidissa</span><span class="sxs-lookup"><span data-stu-id="268c1-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="268c1-103">Microsoft Edge for iOS ja Android sallii käyttäjän selata internetiä useista täysin erillisistä profiileista.</span><span class="sxs-lookup"><span data-stu-id="268c1-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="268c1-104">Microsoft 365:n tietojen laajimmat suojausominaisuudet tulevat saataville, kun tilaat Enterprise Mobility + Security -ohjelmiston, joka sisältää Microsoft Intunen ja Azure Active Directory Premiumin ominaisuudet, kuten ehdollisen käyttöoikeuden.</span><span class="sxs-lookup"><span data-stu-id="268c1-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="268c1-105">Sinun on otettava käyttöön vähintään ehdollinen käyttöoikeuskäytäntö, jonka (1) avulla käyttäjät voivat muodostaa yhteyden mobiililaitteista Microsoft Edge for iOS- ja Android-laitteisiin, ja että (2) toteuttaa Microsoft Intune -sovelluksen suojauskäytännön, joka tarjoaa suojatun selauskokemuksen.</span><span class="sxs-lookup"><span data-stu-id="268c1-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="268c1-106">Lisätietoja ehdollisten accessin ja käytännyjen käytöstä on kohdassa:</span><span class="sxs-lookup"><span data-stu-id="268c1-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="268c1-107">Azure Active Directoryn ehdollisten käyttöoikeuskäytäntöjen käyttö</span><span class="sxs-lookup"><span data-stu-id="268c1-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="268c1-108">Microsoft Intune -sovelluksen suojauskäytäntöjen luominen</span><span class="sxs-lookup"><span data-stu-id="268c1-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="268c1-109">Kertakirjauoinnin käyttäminen Azure Active Directoryssa – yhdistetyt verkkosovellukset käytäntösuojatuissa selaimissa</span><span class="sxs-lookup"><span data-stu-id="268c1-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="268c1-110">Selauskokemuksen hallinta sovelluksen määritysten avulla</span><span class="sxs-lookup"><span data-stu-id="268c1-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="268c1-111">Salli vain työ- ja koulutilien käyttö</span><span class="sxs-lookup"><span data-stu-id="268c1-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="268c1-112">Sovelluksen yleisten määrityskäytäntöjen käyttöönotto</span><span class="sxs-lookup"><span data-stu-id="268c1-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="268c1-113">Sovellusten määrityskäytäntöjen käyttöönotto tietosuojaa varten</span><span class="sxs-lookup"><span data-stu-id="268c1-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="268c1-114">Sovelluksen määrityskäytäntöjen käyttöönotto Microsoft Endpoint Managerin avulla</span><span class="sxs-lookup"><span data-stu-id="268c1-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="268c1-115">Lisätietoja hallittujen sovelluslokien käytöstä on kohdassa Hallittujen sovelluslokien käyttäminen [Microsoft Edge for iOS:](https://go.microsoft.com/fwlink/?linkid=2132578)n ja Androidin avulla.</span><span class="sxs-lookup"><span data-stu-id="268c1-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
