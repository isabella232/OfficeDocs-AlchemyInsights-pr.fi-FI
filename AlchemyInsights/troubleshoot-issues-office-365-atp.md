---
title: Office 365 Advanced Threat Protectionin (ATP) ongelmien vian määritys
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 4164781a331ec919811332e94636449e9d88430d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758062"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="3653a-102">Office 365 ATP:N ongelmien vian määritys</span><span class="sxs-lookup"><span data-stu-id="3653a-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="3653a-103">**Ilmoitettuaan viiveestä Sähkö posti viestin toimituksessa**?</span><span class="sxs-lookup"><span data-stu-id="3653a-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="3653a-104">Kokeile ATP:N turvallisten liite tiedostojen käytäntöjen dynaamista toteutus vaihtoehtoa.</span><span class="sxs-lookup"><span data-stu-id="3653a-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="3653a-105">Näin vältetään Sähkö posti viestien myöhästymis viiveet ja suojataan niitä haitalli silta tiedostoista.</span><span class="sxs-lookup"><span data-stu-id="3653a-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="3653a-106">Haluatko **raportoida väärät positiiviset tai väärät negatiiviset**?</span><span class="sxs-lookup"><span data-stu-id="3653a-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="3653a-107">Käytä tätä linkkiä, kun haluat lähettää tiedoston analyysia varten: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="3653a-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="3653a-108">**Tiesitkö, että voit ottaa käyttöön ATP:N turvallisten linkkien suojauksen Sähkö posti viestissä, joka lähetetään organisaation henkilöiden välillä**?</span><span class="sxs-lookup"><span data-stu-id="3653a-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="3653a-109">Toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="3653a-109">Follow these steps:</span></span>
    1. <span data-ttu-id="3653a-110">Siirry kohtaan https://protection.office.com ja Kirjaudu sisään.</span><span class="sxs-lookup"><span data-stu-id="3653a-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="3653a-111">Siirry **uhkien hallinta**  >  **käytännön**  >  **turvallisiin linkkeihin**.</span><span class="sxs-lookup"><span data-stu-id="3653a-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="3653a-112">Valitse **käytännöt, jotka koskevat tiettyjä käyttäjiä**, Muokkaa (tai lisää) käytäntöä.</span><span class="sxs-lookup"><span data-stu-id="3653a-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="3653a-113">Valitse **Käytä turvallisia linkkejä viesteihin, jotka lähetetään organisaation sisällä**.</span><span class="sxs-lookup"><span data-stu-id="3653a-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="3653a-114">Tallenna käytäntönne ja salli noin 30 minuuttia, ennen kuin muutokset toimivat omassa palvelin keskuksessa.</span><span class="sxs-lookup"><span data-stu-id="3653a-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="3653a-115">Lisä tietoja ATP:N käyttämisestä on kohdassa [Office 365 Advanced Threat Protectionin](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="3653a-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>