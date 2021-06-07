---
title: Microsoft Defender for Endpoint Linuxissa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11490"
- "9001464"
ms.openlocfilehash: 99894d83c51e11ea6dd1746568762eac856306b3
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731452"
---
# <a name="microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="d7407-102">Microsoft Defender for Endpoint Linuxissa</span><span class="sxs-lookup"><span data-stu-id="d7407-102">Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="d7407-103">Yksityiskohtaiset Linux-ohjeet ovat [kohdassa Microsoft Defender for Endpoint Linuxissa.](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux)</span><span class="sxs-lookup"><span data-stu-id="d7407-103">For detailed Linux documentation, see [Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux).</span></span>

<span data-ttu-id="d7407-104">Järjestelmä- ja asennustiedot:</span><span class="sxs-lookup"><span data-stu-id="d7407-104">For system and installation information, see:</span></span>

- [<span data-ttu-id="d7407-105">Ennakkovaatimukset</span><span class="sxs-lookup"><span data-stu-id="d7407-105">Prerequisites</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#prerequisites)
- [<span data-ttu-id="d7407-106">Järjestelmävaatimukset</span><span class="sxs-lookup"><span data-stu-id="d7407-106">System requirements</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#system-requirements)
- [<span data-ttu-id="d7407-107">Asennusohjeet</span><span class="sxs-lookup"><span data-stu-id="d7407-107">Installation instructions</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#installation-instructions)
- [<span data-ttu-id="d7407-108">Verkkoyhteydet</span><span class="sxs-lookup"><span data-stu-id="d7407-108">Network connections</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#network-connections)

<span data-ttu-id="d7407-109">Ohjeita on ohjeaiheissa:</span><span class="sxs-lookup"><span data-stu-id="d7407-109">For instructions, see:</span></span>

- [<span data-ttu-id="d7407-110">Laitteen välityspalvelimen ja Internet-yhteyden asetusten määrittäminen</span><span class="sxs-lookup"><span data-stu-id="d7407-110">Configure device proxy and Internet connectivity settings</span></span>](/microsoft-365/security/defender-endpoint/configure-proxy-internet#enable-access-to-microsoft-defender-atp-service-urls-in-the-proxy-server)
- [<span data-ttu-id="d7407-111">Microsoft Defender for Endpointin päivitysten käyttöönotto Linuxissa</span><span class="sxs-lookup"><span data-stu-id="d7407-111">Deploy updates for Microsoft Defender for Endpoint on Linux</span></span>](/microsoft-365/security/defender-endpoint/linux-updates)
- [<span data-ttu-id="d7407-112">Microsoft Defender for Endpointin määrittäminen Linuxissa</span><span class="sxs-lookup"><span data-stu-id="d7407-112">How to configure Microsoft Defender for Endpoint on Linux</span></span>](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint-linux#how-to-configure-microsoft-defender-for-endpoint-on-linux)
- [<span data-ttu-id="d7407-113">Tuetut komennot</span><span class="sxs-lookup"><span data-stu-id="d7407-113">Supported commands</span></span>](/microsoft-365/security/defender-endpoint/linux-resources#supported-commands)

## <a name="i-need-help"></a><span data-ttu-id="d7407-114">Tarvitsen apua!</span><span class="sxs-lookup"><span data-stu-id="d7407-114">I need help!</span></span>

<span data-ttu-id="d7407-115">Jos et löydä etsimistäsi tiedoista tai ohjeesta, voit tarkentaa haun merkkijonoa.</span><span class="sxs-lookup"><span data-stu-id="d7407-115">If you can't find the information/help you're looking for, refine your search string.</span></span>

<span data-ttu-id="d7407-116">Ennen kuin otat yhteyttä Microsoft-tukeen, muista kerätä ongelman tutkimiseen tarvittavat tiedot ja liittää ne lippuun.</span><span class="sxs-lookup"><span data-stu-id="d7407-116">Before contacting Microsoft Support, make sure to collect the data required to investigate your issue, and attach it to the ticket.</span></span> <span data-ttu-id="d7407-117">Vianmääritystietojen kerääminen on ohjeaiheessa [Diagnostiikkatietojen kerääminen.](/microsoft-365/security/defender-endpoint/linux-resources#collect-diagnostic-information)</span><span class="sxs-lookup"><span data-stu-id="d7407-117">For steps to collect the diagnosic information, see [Collect diagnostic data](/microsoft-365/security/defender-endpoint/linux-resources#collect-diagnostic-information).</span></span>