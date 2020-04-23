---
title: Office 365 Advanced Threat Protection (ATP) -suojausongelmien vianmääritys
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 99bc985f2d66693aca45f0833ab47c043acc1324
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766742"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="aae4b-102">Office 365 ATP:hen liittyvien ongelmien vianmääritys</span><span class="sxs-lookup"><span data-stu-id="aae4b-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="aae4b-103">**Huomaatko viiveet sähköpostiviestin toimittamisessa?**</span><span class="sxs-lookup"><span data-stu-id="aae4b-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="aae4b-104">Kokeile käyttää ATP Safe Attachments -käytäntöjen dynaamista toimitusta -vaihtoehtoa.</span><span class="sxs-lookup"><span data-stu-id="aae4b-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="aae4b-105">Näin vältetään sähköpostiviestien toimitusviiveet ja suojataan vastaanottajia haitallisilta tiedostoilta.</span><span class="sxs-lookup"><span data-stu-id="aae4b-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="aae4b-106">**Haluatko ilmoittaa vääriä positiivisia tai vääriä negatiivisia negatiivisia?**</span><span class="sxs-lookup"><span data-stu-id="aae4b-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="aae4b-107">Tämän linkin avulla voit lähettää tiedoston analyysia varten:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="aae4b-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="aae4b-108">**Tiesitkö, että voit ottaa ATP Safe Links -suojauksen käyttöön organisaation henkilöiden välillä lähetetyille sähköpostiviesteille?**</span><span class="sxs-lookup"><span data-stu-id="aae4b-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="aae4b-109">Toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="aae4b-109">Follow these steps:</span></span>
    1. <span data-ttu-id="aae4b-110">Siirry https://protection.office.comkohtaan ja kirjaudu sisään.</span><span class="sxs-lookup"><span data-stu-id="aae4b-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="aae4b-111">Siirry **Uhkien** > **hallintapolicy** > **Safe Links**.</span><span class="sxs-lookup"><span data-stu-id="aae4b-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="aae4b-112">Muokkaa (tai lisää) käytäntöä **käytännöt, jotka koskevat tiettyjä vastaanottajia.**</span><span class="sxs-lookup"><span data-stu-id="aae4b-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="aae4b-113">Valitse **Käytä turvallisia linkkejä organisaation sisällä lähetettyihin viesteihin**.</span><span class="sxs-lookup"><span data-stu-id="aae4b-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="aae4b-114">Tallenna käytäntö ja anna muutosten kulkea datakeskuksen läpi noin 30 minuuttia.</span><span class="sxs-lookup"><span data-stu-id="aae4b-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="aae4b-115">Lisätietoja ATP:n kanssa on ohjeaiheessa [Office 365 Advanced Threat Protection](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="aae4b-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span></span>