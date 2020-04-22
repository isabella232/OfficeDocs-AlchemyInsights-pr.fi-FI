---
title: 2681 Hyökkäys Simulaattori Microsoft 365:ssä
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
ms.openlocfilehash: 74bd2dd62b24aaf6c9d7b387ab1d97ddab31e902
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713463"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="8819b-102">Hyökkäys Simulator Microsoft 365:ssä</span><span class="sxs-lookup"><span data-stu-id="8819b-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="8819b-103">Kaipaatko Attack Simulatoria?</span><span class="sxs-lookup"><span data-stu-id="8819b-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="8819b-104">Attack Simulator edellyttää **Office 365 Advanced Threat Protection Plan 2:ta (ATP-sopimus 2)** tai **Office 365 Enterprise E5:tä.**</span><span class="sxs-lookup"><span data-stu-id="8819b-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="8819b-105">Attack Simulator **ei** sisälly Office 365 Advanced Threat Protection Plan 1:een (ATP-palvelupaketti 1), Office 365 Enterprise E3:een tai mihinkään Microsoft 365 Apps for Business -tilaukseen.</span><span class="sxs-lookup"><span data-stu-id="8819b-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="8819b-106">Simuloidun hyökkäyksen käynnistämiseen käytettävä tili edellyttää yleisiä järjestelmänvalvojan tai suojauksen järjestelmänvalvojan oikeuksia ja monivaiheista todennusta.The account you use to launch simuloituja hyökkäyksiä edellyttää yleisiä järjestelmänvalvojan tai suojauksen järjestelmänvalvojan oikeuksia ja monivaiheinen todennus (MFA).</span><span class="sxs-lookup"><span data-stu-id="8819b-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="8819b-107">Lisätietoja Attack Simulator -vaatimuksista on [tässä ohjeaiheessa](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span><span class="sxs-lookup"><span data-stu-id="8819b-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="8819b-108">Tärkeää tietoa **Brute Force Salasana** hyökkäys simulaatioita:</span><span class="sxs-lookup"><span data-stu-id="8819b-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="8819b-109">Jos kohdetilillä on mfa käytössä ja salasana on arvattu oikein, tiliä ei näytetä vaarantunut (toinen todennuskerroin on epätäydellinen).</span><span class="sxs-lookup"><span data-stu-id="8819b-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="8819b-110">Salasanatiedosto ei voi olla suurempi kuin 10 Mt.</span><span class="sxs-lookup"><span data-stu-id="8819b-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="8819b-111">Käytä yhtä salasanaa riviä kohden ja sisällytä tyhjä rivi (rivinvaihto) luettelon viimeisen salasanan jälkeen.</span><span class="sxs-lookup"><span data-stu-id="8819b-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="8819b-112">Tärkeitä asioita tietää **Spear Phishing** liittää simulaatioita:</span><span class="sxs-lookup"><span data-stu-id="8819b-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="8819b-113">**Tietojenkalastelun kirjautumispalvelimen URL-osoitteelle**ei voi antaa mukautettua arvoa.</span><span class="sxs-lookup"><span data-stu-id="8819b-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="8819b-114">Jos vastaanottaja käyttää [Ota raporttiviesti käyttöön -apuohjelmaa](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) ilmoittaakseen viestin tietojenkalasteluksi, et ehkä saa ilmoituksia viestistä (koska kyseessä on simuloitu hyökkäys).</span><span class="sxs-lookup"><span data-stu-id="8819b-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="8819b-115">Raportit: Kun simuloitu hyökkäys on valmis, voit tarkastella raporttia valitsemalla **Hyökkäystiedot.**</span><span class="sxs-lookup"><span data-stu-id="8819b-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="8819b-116">Yksityiskohtaiset ohjeet ja uudet ominaisuudet Attack Simulatorissa ovat [ohjeaiheessa Attack Simulator Microsoft 365:ssä](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="8819b-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
