---
title: 2681 Attack Sen Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545723"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="fca8f-102">Attack Attack Attack in Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="fca8f-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="fca8f-103">Puuttuuko Attack Kina?</span><span class="sxs-lookup"><span data-stu-id="fca8f-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="fca8f-104">Attack Defender vaatii **Microsoft Defenderin Office 365 palvelupaketti 2:lle** **tai Office 365 Enterprise E5:lle.**</span><span class="sxs-lookup"><span data-stu-id="fca8f-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="fca8f-105">Attack Defender ei **sisälly** Microsoft Defender for Office 365 Plan 1-, Office 365 Enterprise E3- tai Microsoft 365 -sovellukset yrityksille -tilauksia.</span><span class="sxs-lookup"><span data-stu-id="fca8f-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="fca8f-106">Jäljitettyjen hyökkäysten käynnistämiseen käytettävä tili edellyttää yleisen järjestelmänvalvojan tai suojauksen järjestelmänvalvojan oikeuksia ja monimenetelmäistä todentamista (MFA).</span><span class="sxs-lookup"><span data-stu-id="fca8f-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="fca8f-107">Lisätietoja Attack Kinkin vaatimuksista on [tässä ohjeaiheessa.](/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="fca8f-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="fca8f-108">Tärkeitä asioita, jotka on hyvä tietää **Brute Forcen salasanahyökkäyssimulaatioista:**</span><span class="sxs-lookup"><span data-stu-id="fca8f-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="fca8f-109">Jos kohdetilillä on MFA käytössä ja salasana arvattiin oikein, tili ei näy vaarantumisena (toinen todentamismenetelmä on puutteellinen).</span><span class="sxs-lookup"><span data-stu-id="fca8f-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="fca8f-110">Salasanatiedoston koko voi olla enintään 10 Mt.</span><span class="sxs-lookup"><span data-stu-id="fca8f-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="fca8f-111">Käytä yhtä salasanaa riviä kohti ja lisää tyhjä rivi (rivinvaihto) luettelon viimeisen salasanan jälkeen.</span><span class="sxs-lookup"><span data-stu-id="fca8f-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="fca8f-112">Tärkeitä asioita, jotka on hyvä **tietääphishing-tietokalastelusta** ja simulaatioista:</span><span class="sxs-lookup"><span data-stu-id="fca8f-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="fca8f-113">Tietokalastelun kirjautumispalvelimen URL-osoitteena ei voi olla **mukautettua arvoa.**</span><span class="sxs-lookup"><span data-stu-id="fca8f-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="fca8f-114">Jos vastaanottaja ilmoittaa [](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) viestistä tietojenkalasteluna Ota ilmoita viestistä -apuohjelman käyttöönottajille, et välttämättä saa ilmoituksia viestistä (koska tämä on simuloitu hyökkäys).</span><span class="sxs-lookup"><span data-stu-id="fca8f-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="fca8f-115">Raportit: Kun simuloitu hyökkäys on valmis, voit **tarkastella** raporttia valitsemalla Hyökkäystiedot.</span><span class="sxs-lookup"><span data-stu-id="fca8f-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="fca8f-116">Yksityiskohtaiset ohjeet ja uudet ominaisuudet Attack Attack Attackissa ovat ohjeaiheessa [Attack Sen Microsoft 365.](/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="fca8f-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>
