---
title: Sovellusten yhteensopivuuden testaaminen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9138"
- "9005291"
ms.openlocfilehash: 9a6a9ea3587a851ecf842588ab73421590ce2431
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693658"
---
# <a name="do-app-compatibility-testing"></a><span data-ttu-id="8ba5f-102">Sovellusten yhteensopivuuden testaaminen</span><span class="sxs-lookup"><span data-stu-id="8ba5f-102">Do app compatibility testing</span></span>

<span data-ttu-id="8ba5f-103">Microsoft Edgen sovellusten yhteensopivuus on erittäin suuri.</span><span class="sxs-lookup"><span data-stu-id="8ba5f-103">Application compatibility for Microsoft Edge is extremely high.</span></span> <span data-ttu-id="8ba5f-104">Microsoftin on niin suuri, että se antaa seuraavat yhteensopivuus lupaukset:</span><span class="sxs-lookup"><span data-stu-id="8ba5f-104">In fact, it's so high that Microsoft provides the following compatibility promises:</span></span>
- <span data-ttu-id="8ba5f-105">Jos se toimii Microsoft Edge 45:ssä ja sitä aiemmissa versioissa, se toimii Microsoft Edge 77:ssä ja sitä uudemmassa versiossa.</span><span class="sxs-lookup"><span data-stu-id="8ba5f-105">If it works on Microsoft Edge 45 and earlier versions, it will work on Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="8ba5f-106">Jos se toimii Internet Explorerissa, se toimii Microsoft Edgessä Internet Explorer -tilassa.</span><span class="sxs-lookup"><span data-stu-id="8ba5f-106">If it works on Internet Explorer, it will work on Microsoft Edge in Internet Explorer mode.</span></span>
- <span data-ttu-id="8ba5f-107">Jos se toimii Google Chromessa, se toimii Microsoft Edgessä.</span><span class="sxs-lookup"><span data-stu-id="8ba5f-107">If it works on Google Chrome, it will work on Microsoft Edge.</span></span>

<span data-ttu-id="8ba5f-108">Jos sinulla on sovellus, jossa emme täytä tätä lupausta, pysymme lupauksen takana korjataksesi sen [Microsoft App Assurein avulla.](https://www.microsoft.com/fasttrack/microsoft-365/app-assure)</span><span class="sxs-lookup"><span data-stu-id="8ba5f-108">If you have an application where we don't meet this promise, then we stand behind the promise to fix it with [Microsoft App Assure](https://www.microsoft.com/fasttrack/microsoft-365/app-assure).</span></span>

<span data-ttu-id="8ba5f-109">Lupauksista huolimatta tiedämme, että monien organisaatioiden on vahvistettava sovelluksia yhteensopivuuden tai riskienhallinnan takia.</span><span class="sxs-lookup"><span data-stu-id="8ba5f-109">Despite this promise, we know that many organizations must validate some applications for compliance or risk-management reasons.</span></span> <span data-ttu-id="8ba5f-110">Vaikka olemmekin, että tämä on hyvin yksinkertaista, sovellustestauksen järjestäminen ja järjestäminen on tärkeää.</span><span class="sxs-lookup"><span data-stu-id="8ba5f-110">Even though we expect this to be very straightforward, it's important to be organized and rigorous in app testing.</span></span>

<span data-ttu-id="8ba5f-111">Sovellusten yhteensopivuuden testaamisen voi tehdä kahdella tavalla:</span><span class="sxs-lookup"><span data-stu-id="8ba5f-111">There are two ways to do app compatibility testing:</span></span>

- <span data-ttu-id="8ba5f-112">**Laboratoriotestaus:** Sovellukset testataan tarkasti valvotussa ympäristössä, jossa on tiettyjä määrityksiä.</span><span class="sxs-lookup"><span data-stu-id="8ba5f-112">**Lab testing**: Applications are tested in a tightly controlled environment with specific configurations.</span></span>
- <span data-ttu-id="8ba5f-113">**Pilottikoe:** Sovellukset testataan rajoitetun määrän käyttäjiä päivittäisessä työympäristössä omilla laitteillaan.</span><span class="sxs-lookup"><span data-stu-id="8ba5f-113">**Pilot testing**: Applications are tested by a limited number of users in their daily work environment using their own devices.</span></span>

<span data-ttu-id="8ba5f-114">Valitse kullekin sovellukselle sopivin menetelmä ja testaa ennen koko organisaation käynnistämistä.</span><span class="sxs-lookup"><span data-stu-id="8ba5f-114">Choose the method that is most appropriate for each app and do the testing prior to a launch to the entire organization.</span></span>

<span data-ttu-id="8ba5f-115">Kun olet varmistanut, että sovellukset ovat yhteensopivia, voit ottaa Microsoft Edgen käyttöön pilottiryhmässä.</span><span class="sxs-lookup"><span data-stu-id="8ba5f-115">Once you've ensured that your apps are compatible, you're ready to deploy Microsoft Edge to a pilot group.</span></span>
