---
title: Office 365 Advanced Threat Protection (ATP) -ongelmien vianmääritys
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
ms.openlocfilehash: f1dc675c8a8217ea2824ad46e029bfa303303e6a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511109"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="44940-102">Office 365 ATP:n ongelmien vianmääritys</span><span class="sxs-lookup"><span data-stu-id="44940-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="44940-103">**Ilmoitus viivästyksiä sähköpostiviestin toimitus?**</span><span class="sxs-lookup"><span data-stu-id="44940-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="44940-104">Kokeile ATP Safe Attachments -käytäntöjen Dynaaminen toimitus -vaihtoehtoa.</span><span class="sxs-lookup"><span data-stu-id="44940-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="44940-105">Näin vältetään sähköpostiviestien toimitusviiveet ja suojataan vastaanottajia haitallisilta tiedostoilta.</span><span class="sxs-lookup"><span data-stu-id="44940-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="44940-106">**Haluatko ilmoittaa vääriä positiivisia tai vääriä negatiivisia negatiivisia?**</span><span class="sxs-lookup"><span data-stu-id="44940-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="44940-107">Tämän linkin avulla voit lähettää tiedoston analysoitavaksi:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="44940-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="44940-108">**Tiesitkö, että voit ottaa ATP Safe Links -suojauksen käyttöön organisaatiosi ihmisten välillä lähetetyille sähköpostiviesteille?**</span><span class="sxs-lookup"><span data-stu-id="44940-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="44940-109">Toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="44940-109">Follow these steps:</span></span>
    1. <span data-ttu-id="44940-110">Siirry https://protection.office.com ja kirjaudu sisään.</span><span class="sxs-lookup"><span data-stu-id="44940-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="44940-111">Siirry **Uhkien**  >  **hallintakäytäntö**  >  **Turvalliset linkit**.</span><span class="sxs-lookup"><span data-stu-id="44940-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="44940-112">Muokkaa (tai lisää) käytäntöä Koskevat käytännöt -kohdassa **Käytännöt, jotka koskevat tiettyjä vastaanottajia.**</span><span class="sxs-lookup"><span data-stu-id="44940-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="44940-113">Valitse **Käytä turvallisia linkkejä organisaation sisällä lähetettyihin viesteihin**.</span><span class="sxs-lookup"><span data-stu-id="44940-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="44940-114">Tallenna käytäntösi ja anna muutosten toimia palvelinkeskuksen läpi noin 30 minuuttia.</span><span class="sxs-lookup"><span data-stu-id="44940-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="44940-115">Lisätietoja ATP:n kanssa on [ohjeaiheessa Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="44940-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>