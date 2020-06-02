---
title: 2681 Hyökkäyssimulaattori Microsoft 365:ssä
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 3dae4768ca62757ce7f92dfc527078c963d72742
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506735"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="53cd0-102">Hyökkäyssimulaattori Microsoft 365:ssä</span><span class="sxs-lookup"><span data-stu-id="53cd0-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="53cd0-103">Puuttuuko Attack Simulator?</span><span class="sxs-lookup"><span data-stu-id="53cd0-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="53cd0-104">Attack Simulator edellyttää **Office 365 Advanced Threat Protection Plan 2:ta (ATP-palvelupaketti 2)** tai **Office 365 Enterprise E5:tä.**</span><span class="sxs-lookup"><span data-stu-id="53cd0-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="53cd0-105">Attack Simulator **ei** sisälly Office 365 Advanced Threat Protection Plan 1:een (ATP-palvelupaketti 1), Office 365 Enterprise E3:een tai mihinkään Microsoft 365 -sovellukseen yrityksille -tilauksiin.</span><span class="sxs-lookup"><span data-stu-id="53cd0-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="53cd0-106">Simuloitujen hyökkäysten käynnistämiseen käytettävä tili edellyttää yleisen järjestelmänvalvojan tai suojauksen järjestelmänvalvojan oikeuksia ja mfa-todennusta.</span><span class="sxs-lookup"><span data-stu-id="53cd0-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="53cd0-107">Lisätietoja Attack Simulator -vaatimuksista on [tässä ohjeaiheessa](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="53cd0-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="53cd0-108">Tärkeitä asioita tietää **Brute Force Password** hyökkäys simulaatiot:</span><span class="sxs-lookup"><span data-stu-id="53cd0-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="53cd0-109">Jos kohdetilillä on mfa käytössä ja salasana on arvattu oikein, tiliä ei näy vaarantuneena (toinen todennuskerroin on epätäydellinen).</span><span class="sxs-lookup"><span data-stu-id="53cd0-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="53cd0-110">Salasanatiedoston koko ei voi olla suurempi kuin 10 Mt.</span><span class="sxs-lookup"><span data-stu-id="53cd0-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="53cd0-111">Käytä yhtä salasanaa riviä kohden ja lisää tyhjä rivi (rivinvaihto) luettelon viimeisen salasanan jälkeen.</span><span class="sxs-lookup"><span data-stu-id="53cd0-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="53cd0-112">Tärkeitä asioita, jotka on tiedettävä **Spear Phishing** -liittääksesi simulaatioita:</span><span class="sxs-lookup"><span data-stu-id="53cd0-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="53cd0-113">Et voi antaa mukautettua arvoa **tietojenkalastelun kirjautumispalvelimen URL-osoitteelle.**</span><span class="sxs-lookup"><span data-stu-id="53cd0-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="53cd0-114">Jos vastaanottaja ilmoittaa viestin tietojenkalasteluksi [Ota raporttiviesti käyttöön -apuohjelman](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) avulla, et ehkä saa ilmoituksia viestistä (koska kyseessä on simuloitu hyökkäys).</span><span class="sxs-lookup"><span data-stu-id="53cd0-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="53cd0-115">Raportit: Kun simuloitu hyökkäys on valmis, voit tarkastella raporttia valitsemalla **Hyökkäyksen tiedot.**</span><span class="sxs-lookup"><span data-stu-id="53cd0-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="53cd0-116">Lisätietoja Attack Simulatorin yksityiskohtaisista ohjeista ja uusista ominaisuuksista on [ohjeaiheessa Attack Simulator Microsoft 365 :ssä](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="53cd0-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
