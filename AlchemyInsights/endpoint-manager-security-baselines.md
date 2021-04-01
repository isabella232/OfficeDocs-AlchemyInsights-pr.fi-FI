---
title: EndPointin hallinta – Suojauksen perustasot
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
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440881"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="66e19-102">EndPointin hallinta – Suojauksen perustasot</span><span class="sxs-lookup"><span data-stu-id="66e19-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="66e19-103">Suojauksen perustasot ovat valmiiksi määritettyjä Windows-asetusryhmiä, joiden avulla voit ottaa käyttöön niitä suojausasetuksia, joita asianomaiset suojausryhmät suosittelevat.</span><span class="sxs-lookup"><span data-stu-id="66e19-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="66e19-104">Näitä perustasoja voidaan mukauttaa toimittamaan vain halutut asetukset ja arvot.</span><span class="sxs-lookup"><span data-stu-id="66e19-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="66e19-105">Lisätietoja suojauksen perustasoista on ohjeaiheessa [Windows 10 -laitteiden määrittäminen Intunessa](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="66e19-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="66e19-106">Perustasoja on tällä hetkellä näissä tuotteissa:</span><span class="sxs-lookup"><span data-stu-id="66e19-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="66e19-107">Windows mobiililaitteidenhallinen suojausasetukset</span><span class="sxs-lookup"><span data-stu-id="66e19-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="66e19-108">Microsoft Defender for EndPoint Security</span><span class="sxs-lookup"><span data-stu-id="66e19-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="66e19-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="66e19-109">Microsoft Edge</span></span>

<span data-ttu-id="66e19-110">Jokainen perustaso päivitetään säännöllisesti ja julkaistaan asteittaisina versioina.</span><span class="sxs-lookup"><span data-stu-id="66e19-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="66e19-111">Jokainen versio lisää ja poistaa edellisestä versiosta asetuksia sen varmistamiseksi, että perustaso täyttää nykyiset ohjeet.</span><span class="sxs-lookup"><span data-stu-id="66e19-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="66e19-112">Päätepisteen suojauksen perustason konsoli sallii eri versioiden vertailun tekemällä muutokset versiosta versioon näkyviksi.</span><span class="sxs-lookup"><span data-stu-id="66e19-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="66e19-113">Ohjeita siitä, miten voit tehokkaasti muuttaa sitä, mikä perustason versio on käytössä, on kohdassa [Suojauksen perustason profiilien hallinta Microsoft Intunessa](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="66e19-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="66e19-114">Kun olet ottanut suojauksen perustasokäyttöön, voit valvoa käyttöönoton tilaa ja tarkastella asetuksia laitekohtaisesti.</span><span class="sxs-lookup"><span data-stu-id="66e19-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="66e19-115">**Huomautus:** Perustasojen raportointitietojen tuleminen näkyviin ensimmäisen käyttöönoton jälkeen laitteeseen voi kestää jopa 24 tuntia ja lisäpäivityksiä varten enintään 6 tuntia.</span><span class="sxs-lookup"><span data-stu-id="66e19-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="66e19-116">Yleisin syy perustason määrittämisen epäonnistumiseen on, että samaa asetusta käytetään eri profiilissa.</span><span class="sxs-lookup"><span data-stu-id="66e19-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="66e19-117">Tämä skenaario voidaan tutkia tietyssä laitteessa valitsemalla tämä laite Suojauksen perustaso -profiilin Laitteen tila -solmusta.</span><span class="sxs-lookup"><span data-stu-id="66e19-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="66e19-118">Lisätietoja on kohdassa [Suojauksen perustasojen ristiriitojen ratkaiseminen](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="66e19-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>