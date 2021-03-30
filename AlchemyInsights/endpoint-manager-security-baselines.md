---
title: EndPoint Manager – suojauksen perusaikataulut
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/29/2021
ms.locfileid: "51420878"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="21366-102">EndPoint Manager – suojauksen perusaikataulut</span><span class="sxs-lookup"><span data-stu-id="21366-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="21366-103">Suojauksen perusaikataulut ovat valmiiksi määritettyjä Windows-asetusryhmiä, joiden avulla voit ottaa käyttöön asianomaisten suojausryhmien suosittelemia suojausasetuksia.</span><span class="sxs-lookup"><span data-stu-id="21366-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="21366-104">Näitä perusaikatauluja voidaan mukauttaa toimittamaan vain halutut asetukset ja arvot.</span><span class="sxs-lookup"><span data-stu-id="21366-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="21366-105">Lisätietoja suojauksen perusaikatauluista on ohjeaiheessa Windows 10 -laitteiden määrittäminen [Intunessa suojauksen perusaikataulujen avulla.](https://docs.microsoft.com/mem/intune/protect/security-baselines)</span><span class="sxs-lookup"><span data-stu-id="21366-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="21366-106">Näiden tuotteiden perusaikatauluja on tällä hetkellä:</span><span class="sxs-lookup"><span data-stu-id="21366-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="21366-107">Windowsin MDM-suojausasetukset</span><span class="sxs-lookup"><span data-stu-id="21366-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="21366-108">Microsoft Defender for EndPoint Security</span><span class="sxs-lookup"><span data-stu-id="21366-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="21366-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="21366-109">Microsoft Edge</span></span>

<span data-ttu-id="21366-110">Kukin perusaikataulu päivitetään säännöllisesti ja julkaistaan asteittain.</span><span class="sxs-lookup"><span data-stu-id="21366-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="21366-111">Kukin versio lisää ja poistaa edellisestä versiosta asetukset sen varmistamiseksi, että perusaikataulu vastaa nykyisiä ohjeita.</span><span class="sxs-lookup"><span data-stu-id="21366-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="21366-112">Päätepisteen suojauksen perussolsoleiden avulla eri versioita voidaan verrata tekemällä muutokset versiosta versioon näkyvissä.</span><span class="sxs-lookup"><span data-stu-id="21366-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="21366-113">Ohjeita perusaikataulun käyttöönottoversion tehokkaimpaan muutokseen on Kohdassa Suojauksen perusaikataulun profiilien hallinta [Microsoft Intunessa.](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)</span><span class="sxs-lookup"><span data-stu-id="21366-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="21366-114">Kun olet ottanut suojauksen perusaikataulun käyttöön, voit valvoa käyttöönoton tila ja tarkistaa asetukset laitekohtaisesti.</span><span class="sxs-lookup"><span data-stu-id="21366-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="21366-115">**Huomautus:** Perusaikataulujen raportointitiedot voivat näkyä 24 tunnin kuluessa käyttöönotosta laitteeseen ja enintään 6 tuntia lisäpäivityksiä varten.</span><span class="sxs-lookup"><span data-stu-id="21366-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="21366-116">Perusaikataulun asetuksen ei yleensä tarvitse olla käytössä, koska samaa asetusta käytetään eri profiilissa.</span><span class="sxs-lookup"><span data-stu-id="21366-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="21366-117">Voit tutkia tätä skenaariota tietyssä laitteessa valitsemalla laitteen Security Baseline -profiilin Laitteen tila -solmussa.</span><span class="sxs-lookup"><span data-stu-id="21366-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="21366-118">Lisätietoja on kohdassa [Suojauksen perusaikataulujen ristiriitojen ratkaiseminen.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)</span><span class="sxs-lookup"><span data-stu-id="21366-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>