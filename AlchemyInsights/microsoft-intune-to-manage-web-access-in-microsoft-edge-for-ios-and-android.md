---
title: Microsoft Intunen käyttäminen verkko käytön hallintaan Microsoft Edgessä iOS:ssä ja Androidissa
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
ms.openlocfilehash: 4d6ab4df4ff9588ce5052421602e347c76c91c3f
ms.sourcegitcommit: a7952283882d341515623d5ae58eda14d0553449
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/10/2020
ms.locfileid: "49678256"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="c244a-102">Microsoft Intunen käyttäminen verkko käytön hallintaan Microsoft Edgessä iOS:ssä ja Androidissa</span><span class="sxs-lookup"><span data-stu-id="c244a-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="c244a-103">Microsoft Edge for iOS:n ja Androidin avulla käyttäjä voi selata Internetiä useista täysin erillisistä profiileista.</span><span class="sxs-lookup"><span data-stu-id="c244a-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="c244a-104">Microsoft 365-tietojen laajimman suojaus ominaisuudet ovat käytettävissä, kun tilaat Enterprise Mobility +-tieto turva paketin, joka sisältää Microsoft Intune-ja Azure Active Directory Premium-ominaisuudet, kuten ehdollisen käyttö oikeuden.</span><span class="sxs-lookup"><span data-stu-id="c244a-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="c244a-105">Vähintään, sinun kannattaa ottaa käyttöön ehdollinen käyttö oikeus menettely, joka (1) sallii käyttäjien muodostaa yhteyden mobiililaitteista Microsoft Edge for iOS:ään ja Androidiin, ja että (2) toteuttaa Microsoft Intune-sovelluksen suojaus käytäntöä, joka tarjoaa suojatun selaus kokemuksen.</span><span class="sxs-lookup"><span data-stu-id="c244a-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="c244a-106">Lisä tietoja ehdollisen käytön ja käytäntöjen käyttämisestä on artikkeleissa:</span><span class="sxs-lookup"><span data-stu-id="c244a-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="c244a-107">Azure Active Directoryn ehdollisen käytön käytäntöjen käyttäminen</span><span class="sxs-lookup"><span data-stu-id="c244a-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="c244a-108">Microsoft Intune-sovelluksen suojaus käytäntöjen luominen</span><span class="sxs-lookup"><span data-stu-id="c244a-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="c244a-109">Kertakirjautumisen käyttäminen Azure Active Directoryssa – yhdistetyt verkko sovellukset käytäntöjen suojaavissa selaimissa</span><span class="sxs-lookup"><span data-stu-id="c244a-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="c244a-110">Selaus kokemuksen hallinta sovelluksen määritysten avulla</span><span class="sxs-lookup"><span data-stu-id="c244a-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="c244a-111">Salli vain työ-ja koulu-tunnusten käyttö</span><span class="sxs-lookup"><span data-stu-id="c244a-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="c244a-112">Yleisten sovelluksen määritys käytäntöjen käyttöönotto</span><span class="sxs-lookup"><span data-stu-id="c244a-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="c244a-113">Sovelluksen määritys käytäntöjen käyttöönotto tieto suojausta varten</span><span class="sxs-lookup"><span data-stu-id="c244a-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="c244a-114">Sovellusten määritys käytäntöjen käyttöönottaminen Microsoft Endpoint Managerillä</span><span class="sxs-lookup"><span data-stu-id="c244a-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="c244a-115">Lisä tietoja hallittujen sovellus lokien käyttämisestä on artikkelissa [Hallittujen sovellus lokien käyttö Microsoft Edge for iOS:ssä ja Androidissa](https://go.microsoft.com/fwlink/?linkid=2132578).</span><span class="sxs-lookup"><span data-stu-id="c244a-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
