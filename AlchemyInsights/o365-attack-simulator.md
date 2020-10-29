---
title: 2681-hyökkäys simulaattori Microsoft 365-sovelluksessa
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
ms.openlocfilehash: 7b48abea3400e3565f2ba33c97e24e5b9923eb3b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801548"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="e6b0d-102">Hyökkäys simulaattori Microsoft 365-sovelluksessa</span><span class="sxs-lookup"><span data-stu-id="e6b0d-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="e6b0d-103">Oletko puuttuvasta hyökkäys simulaattorista?</span><span class="sxs-lookup"><span data-stu-id="e6b0d-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="e6b0d-104">Hyökkäys simulaattori edellyttää **Microsoft Defender for office 365-ohjelmaa (ATP-sopimus 2)** tai **Office 365 Enterprise-E5** .</span><span class="sxs-lookup"><span data-stu-id="e6b0d-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5** .</span></span> <span data-ttu-id="e6b0d-105">Hyökkäys simulaattori ei **sisälly Microsoft** Defender for Office 365-pakettiin (ATP-Paketti 1), Office 365 Enterprise E3-ohjelmaan tai mihinkään Microsoft 365-sovellukseen yritys tilauksia varten.</span><span class="sxs-lookup"><span data-stu-id="e6b0d-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="e6b0d-106">Tili, jota käytät simuloitujen hyökkäysten käynnistämiseen, edellyttää yleisten järjestelmänvalvojien tai suojaus järjestelmänvalvojien käyttö oikeuksia ja usean tekijän todennusta.</span><span class="sxs-lookup"><span data-stu-id="e6b0d-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="e6b0d-107">Lisä tietoja hyökkäys simulaattori vaatimuksista on [tässä](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)artikkelissa.</span><span class="sxs-lookup"><span data-stu-id="e6b0d-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="e6b0d-108">Tärkeitä huomioitavia asioita **Brute Force-Sala sanan** hyökkäys simulaatioista:</span><span class="sxs-lookup"><span data-stu-id="e6b0d-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="e6b0d-109">Jos kohde tilillä on käytössä MFA ja sala sana on oikein, tili ei näy vaarantuneen (toinen todennus kerroin on epätäydellinen).</span><span class="sxs-lookup"><span data-stu-id="e6b0d-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="e6b0d-110">Salasana tiedosto ei voi olla suurempi kuin 10 Mt.</span><span class="sxs-lookup"><span data-stu-id="e6b0d-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="e6b0d-111">Käytä yhtä riviä kohden Sala sanaa ja Sisällytä tyhjä rivi (rivin vaihto) luettelon viimeisen Sala sanan perään.</span><span class="sxs-lookup"><span data-stu-id="e6b0d-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="e6b0d-112">Tärkeitä asioita, jotka on hyvä tietää **Spear phishing** Liitä-simulaatioista:</span><span class="sxs-lookup"><span data-stu-id="e6b0d-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="e6b0d-113">Et voi määrittää mukautettua arvoa **tietojen kalastelu-kirjautumispalvelimen URL-osoitteille** .</span><span class="sxs-lookup"><span data-stu-id="e6b0d-113">By design, you can't provide a custom value for **Phishing login server URL** .</span></span>

  - <span data-ttu-id="e6b0d-114">Jos vastaanottajalla on käytössä [Ilmoita viestistä-apuohjelma](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) , joka ilmoittaa viestin tietojenkalasteluksi, et ehkä saa ilmoituksia viestistä (koska kyseessä on simuloitu hyökkäys).</span><span class="sxs-lookup"><span data-stu-id="e6b0d-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="e6b0d-115">Raportit: kun simuloitu hyökkäys on valmis, voit tarkastella raporttia napsauttamalla **hyökkäys tiedot** -painiketta.</span><span class="sxs-lookup"><span data-stu-id="e6b0d-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="e6b0d-116">Yksityiskohtaisia ohjeita ja hyökkäys simulaattorin uusia ominaisuuksia on artikkelissa [hyökkäys simulaattori Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)-sovelluksessa.</span><span class="sxs-lookup"><span data-stu-id="e6b0d-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
