---
title: 2681 hyökkäys simulaattori Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/27/2019
ms.locfileid: "37305329"
---
# <a name="attack-simulator-in-office-365"></a><span data-ttu-id="b74cc-102">Hyökkäys simulaattori Office 365</span><span class="sxs-lookup"><span data-stu-id="b74cc-102">Attack Simulator in Office 365</span></span>

- <span data-ttu-id="b74cc-103">Puuttuuko hyökkäys simulaattori?</span><span class="sxs-lookup"><span data-stu-id="b74cc-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="b74cc-104">Hyökkäys simulaattori edellyttää **office 365 Advanced uhkien torjunta suunnitelma 2 (ATP-suunnitelma 2)** tai **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="b74cc-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="b74cc-105">Hyökkäys simulaattori **ei** sisälly Office 365 Advanced Threat Protection-suunnitelmaan 1 (ATP-suunnitelma 1), Office 365 Enterprise E3-yritykseen tai mihin tahansa Office 365-yritys tilauksiin.</span><span class="sxs-lookup"><span data-stu-id="b74cc-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Office 365 Business subscriptions.</span></span>

- <span data-ttu-id="b74cc-106">Simuloitujen hyökkäysten käynnistämiseen käytettävä tili edellyttää yleisen järjestelmänvalvojan tai suoja uksen järjestelmänvalvojan oikeuksia ja monimitostodennusta (MFA).</span><span class="sxs-lookup"><span data-stu-id="b74cc-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="b74cc-107">Lisä tietoja hyökkäys simulaattorin vaatimuksista [on tässä ohje aiheessa](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span><span class="sxs-lookup"><span data-stu-id="b74cc-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="b74cc-108">Tärkeitä asioita tietää **Brute Force sala sana** hyökkäys simulaatiot:</span><span class="sxs-lookup"><span data-stu-id="b74cc-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="b74cc-109">Jos kohde tili on MFA käytössä ja sala sana on arvattu oikein, tiliä ei näy vaarantuneeksi (toinen todennus kerroin on puutteellinen).</span><span class="sxs-lookup"><span data-stu-id="b74cc-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="b74cc-110">Salasana tiedoston koko ei voi olla suurempi kuin 10 Mt.</span><span class="sxs-lookup"><span data-stu-id="b74cc-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="b74cc-111">Käytä yksi sala sana riviä kohden ja Sisällytä tyhjä rivi (rivin tuotto) luettelon viimeisen Sala sanan jälkeen.</span><span class="sxs-lookup"><span data-stu-id="b74cc-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="b74cc-112">Tärkeitä asioita tietää **Spear phishing** Liitä simulaatiot:</span><span class="sxs-lookup"><span data-stu-id="b74cc-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="b74cc-113">Et voi antaa mukautettua arvoa **tietojen kalastelun torjunta palvelimen URL-osoitteelle**.</span><span class="sxs-lookup"><span data-stu-id="b74cc-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="b74cc-114">Jos vastaanottaja ilmoittaa sanoman tietojenkalasteluksi [Ota käyttöön raportti viesti-apuohjelman](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) avulla, et ehkä saa ilmoituksia viestistä (koska kyseessä on simuloitu hyökkäys).</span><span class="sxs-lookup"><span data-stu-id="b74cc-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="b74cc-115">Raportit: kun simuloitu hyökkäys on valmis, voit napsauttaa **hyökkäys tiedot** nähdäksesi raportin.</span><span class="sxs-lookup"><span data-stu-id="b74cc-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="b74cc-116">Tarkempia ohjeita ja uusia ominaisuuksia hyökkäys simulaattori, katso [hyökkäys simulaattori Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="b74cc-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
