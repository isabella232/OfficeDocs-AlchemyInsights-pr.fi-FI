---
title: Microsoft Edgen tuki Microsoft Defender Application Guard-sovellukselle
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583585"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a><span data-ttu-id="08544-102">Microsoft Edgen tuki Microsoft Defender Application Guard-sovellukselle</span><span class="sxs-lookup"><span data-stu-id="08544-102">Microsoft Edge's support for Microsoft Defender Application Guard</span></span>

<span data-ttu-id="08544-103">Windows 10: lle ja Microsoft Edgelle suunniteltu Application Guard käyttää laitteistoeristämis tapaa, jonka avulla käyttäjä voi siirtyä epäluotettavaan sivustoon, joka on erotettu isäntä käyttö järjestelmästä.</span><span class="sxs-lookup"><span data-stu-id="08544-103">Designed for Windows 10 and Microsoft Edge, Application Guard uses a hardware-isolation approach that lets a user navigate an untrusted site from inside an isolated, Hyper-V–enabled container, separated from the host operating system.</span></span>

<span data-ttu-id="08544-104">Yrityksen järjestelmänvalvoja määrittää luotettujen sivustojen, pilvi resurssien ja sisäisten verkkojen luettelon.</span><span class="sxs-lookup"><span data-stu-id="08544-104">An enterprise admin defines a list of trusted websites, cloud resources, and internal networks.</span></span> <span data-ttu-id="08544-105">Kun käyttäjä vierailee sivustossa, joka ei ole luettelossa, Microsoft Edge Avaa sivuston säilöön.</span><span class="sxs-lookup"><span data-stu-id="08544-105">When a user visits a site that's not on the list, Microsoft Edge will open the site in the container.</span></span> <span data-ttu-id="08544-106">Tämä tarkoittaa, että jos sivusto osoittautuu haitalli seksi, isäntä tieto kone säilyy suojattuna eikä hyökkääjä pääse yritys tietoihin.</span><span class="sxs-lookup"><span data-stu-id="08544-106">This means that if the site turns out to be malicious, the host PC will remain protected and the attacker won't get to the enterprise data.</span></span>

<span data-ttu-id="08544-107">Säilön laajennusten asentamista tuetaan Microsoft Edge-version 81 kautta, ja sitä voidaan hallita käytännöllä.</span><span class="sxs-lookup"><span data-stu-id="08544-107">Installation of extensions in the container is supported as of Microsoft Edge version 81, and it can be controlled via a policy.</span></span> <span data-ttu-id="08544-108">Extensioninstallfortecelist-käytännöllä käytettävä updateURL-osoite lisätään neutraalina resurssina Application Guard-sovelluksen käyttämissä verkon eristys politiikoissa.</span><span class="sxs-lookup"><span data-stu-id="08544-108">The updateURL address that gets used in the ExtensionInstallForcelist policy should be added as a Neutral Resource in the Network Isolation policies used by Application Guard.</span></span>

<span data-ttu-id="08544-109">Lisä tietoja on Ohje aiheessa Microsoft [Edge-tuki Microsoft Defender Application Guard-sovellukselle](https://go.microsoft.com/fwlink/?linkid=2134229).</span><span class="sxs-lookup"><span data-stu-id="08544-109">For more info, see [Microsoft Edge support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span></span>
