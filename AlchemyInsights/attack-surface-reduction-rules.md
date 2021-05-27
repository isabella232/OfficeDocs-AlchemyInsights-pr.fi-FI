---
title: Hyökkäyspinta-alalle vähennyssäännöt
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676230"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="029e4-102">Hyökkäyspinta-alalle vähennyssäännöt</span><span class="sxs-lookup"><span data-stu-id="029e4-102">Attack surface reduction rules</span></span>

<span data-ttu-id="029e4-103">Tiedostojen tai kansioiden poissulkeminen voi heikentää merkittävästi hyökkäyspinta-alalle vähennyssääntöjen suojausta.</span><span class="sxs-lookup"><span data-stu-id="029e4-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="029e4-104">Tiedostot, jotka sääntö olisi estänyt, ovat sallittuja, eikä raporttia tai tapahtumaa tallenneta.</span><span class="sxs-lookup"><span data-stu-id="029e4-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="029e4-105">Poikkeus koskee kaikkia sääntöjä, jotka sallivat poikkeukset.</span><span class="sxs-lookup"><span data-stu-id="029e4-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="029e4-106">ASR-poikkeukset käyttävät samaa syntaksia kuin Microsoft Defenderin virustentorjunta poissulkemiset.</span><span class="sxs-lookup"><span data-stu-id="029e4-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="029e4-107">Lisätietoja on kohdassa [Poikkeuksien määrittäminen ja vahvistaminen Microsoft Defenderin virustentorjunta tarkistamista varten.](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="029e4-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="029e4-108">Voit välttää ongelmat tutustumaan yleisiin virheisiin, joita on [syytä välttää poissulkemista määrittäessä.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="029e4-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="029e4-109">Kaikki ASR-säännöt eivät tue poikkeuksia.</span><span class="sxs-lookup"><span data-stu-id="029e4-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="029e4-110">Jos haluat tarkistaa, tukeeko sääntö poikkeuksia, tutustu taulukkoon [Hyökkäyspinta-ala-vähennyssäännöt](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="029e4-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="029e4-111">Hyökkäyspinta-alalle vähennyssäännöt</span><span class="sxs-lookup"><span data-stu-id="029e4-111">Attack surface reduction rules</span></span>

<span data-ttu-id="029e4-112">Organisaatiosi hyökkäyspinta sisältää kaikki paikat, joissa hyökkäykset voivat vaarantaa organisaation laitteita tai verkkoja.</span><span class="sxs-lookup"><span data-stu-id="029e4-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="029e4-113">Hyökkäyspinta-alasi pienentäminen tarkoittaa organisaation laitteiden ja verkon suojaamista, jolloin hyökkäykset voidaan suorittaa vähempään eri tavalla.</span><span class="sxs-lookup"><span data-stu-id="029e4-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="029e4-114">Hyökkäyspinta-alaan pienentämistä koskevien sääntöjen määrittäminen Microsoft Defender for Endpointissa voi auttaa.</span><span class="sxs-lookup"><span data-stu-id="029e4-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="029e4-115">Lisätietoja on seuraavissa artikkeleissa:</span><span class="sxs-lookup"><span data-stu-id="029e4-115">For more information, see:</span></span>

- [<span data-ttu-id="029e4-116">Yhdistä ASR-säännön GUID nimeksi</span><span class="sxs-lookup"><span data-stu-id="029e4-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="029e4-117">ASR-sääntöjen vaatimukset:</span><span class="sxs-lookup"><span data-stu-id="029e4-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="029e4-118">Windows 10 Pro, versio 1709 tai uudempi</span><span class="sxs-lookup"><span data-stu-id="029e4-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="029e4-119">Windows 10 Enterprise versio 1709 tai uudempi</span><span class="sxs-lookup"><span data-stu-id="029e4-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="029e4-120">Windows Palvelin, versio 1803 (puolivuosittainen kanava) tai uudempi</span><span class="sxs-lookup"><span data-stu-id="029e4-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="029e4-121">Oikean poissulkemisen tunnistaminen</span><span class="sxs-lookup"><span data-stu-id="029e4-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="029e4-122">Etsi tapahtumatunnus 1121 tai 1122 Microsoft-Windows-Windows Defender/toimintalokista.</span><span class="sxs-lookup"><span data-stu-id="029e4-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="029e4-123">Arvioi lohkoskenaario ja -konteksti ja varmista, että tämän skenaarion esto on avattava.</span><span class="sxs-lookup"><span data-stu-id="029e4-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="029e4-124">Lue Tapahtuman tietojen Polku-arvo, joka on poissulkemisen määrittävä arvo.</span><span class="sxs-lookup"><span data-stu-id="029e4-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="029e4-125">Tee poissulkemisista mahdollisimman tarkkoja.</span><span class="sxs-lookup"><span data-stu-id="029e4-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="029e4-126">Käytä tarvittaessa yleismerkkiä (esimerkiksi korvaa käyttäjämuuttuja).</span><span class="sxs-lookup"><span data-stu-id="029e4-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="029e4-127">Ota poikkeus käyttöön käyttöönottotarpeiden mukaan.</span><span class="sxs-lookup"><span data-stu-id="029e4-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="029e4-128">Lisätietoja on ohjeaiheessa [Hyökkäyspinta-alaan pienentämistä koskevien sääntöjen mukauttaminen.](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)</span><span class="sxs-lookup"><span data-stu-id="029e4-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="029e4-129">Poissulkemista ei poisteta</span><span class="sxs-lookup"><span data-stu-id="029e4-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="029e4-130">Määritä, tukeeko sääntö poikkeuksia.</span><span class="sxs-lookup"><span data-stu-id="029e4-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="029e4-131">Lisätietoja on kohdassa [Hyökkäyspinta-alaan pienentämistä koskevat säännöt](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="029e4-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="029e4-132">Tarkista poikkeukset ja tarkista, onko tapahtumassa käytetty kirjoitusvirheitä tai väärin kirjoitettuja yleismerkkejä.</span><span class="sxs-lookup"><span data-stu-id="029e4-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="029e4-133">Lisätietoja on kohdassa Tuetut [poikkeustyypit](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="029e4-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="029e4-134">Jos säännön vaikutus on liian suuri, harkitse säännön (takaisin) siirtäminen Valvonta-tilaan lisätarkistusta varten.</span><span class="sxs-lookup"><span data-stu-id="029e4-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="029e4-135">Lisätietoja on kohdassa [Testaa, miten Microsoft Defender for Endpoint -ominaisuudet toimivat valvontatilassa.](/microsoft-365/security/defender-endpoint/audit-windows-defender)</span><span class="sxs-lookup"><span data-stu-id="029e4-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="029e4-136">Kerää tukitietoja tukitapauksen a avaamista varten tällä komennolla:</span><span class="sxs-lookup"><span data-stu-id="029e4-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="029e4-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="029e4-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="029e4-138">Lisätietoja on kohdassa Ongelmia Microsoft [Defender for Endpointsissa onboarding-koneissa.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="029e4-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
