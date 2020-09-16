---
title: Päivittäinen sähkö postin enimmäismäärä ylittyi. Työn kulku on odotus tilassa.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731560"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="6f315-103">Päivittäinen sähkö postin enimmäismäärä ylittyi.</span><span class="sxs-lookup"><span data-stu-id="6f315-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="6f315-104">Työn kulku on odotus tilassa.</span><span class="sxs-lookup"><span data-stu-id="6f315-104">Workflow is suspended.</span></span>

<span data-ttu-id="6f315-105">Tämä virhe saattaa tulla näyttöön seuraavissa tilanteissa:</span><span class="sxs-lookup"><span data-stu-id="6f315-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="6f315-106">Sinulla on SharePoint Onlinen työn kulku, joka käyttää SharePoint 2010-tai SharePoint 2013-työn kulku ympäristön tyyppiä.</span><span class="sxs-lookup"><span data-stu-id="6f315-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="6f315-107">Työn kulku on määritetty lähettämään mukautettu Sähkö posti viesti useammalle kuin 200-käyttäjälle kerralla, yli 10 000 käyttäjää päivässä tai yli 30 viestiä minuutissa.</span><span class="sxs-lookup"><span data-stu-id="6f315-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="6f315-108">Kun suoritat työn kulun, sähkö posti viestiä ei lähetetä ja huomaat seuraavan ongelman:</span><span class="sxs-lookup"><span data-stu-id="6f315-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="6f315-109">Jos käytät työn kulkua SharePoint 2013-ympäristö tyypin kanssa, Selaa **työn kulun tila** -sivulle.</span><span class="sxs-lookup"><span data-stu-id="6f315-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="6f315-110">Työn kulun tila-sivulla **sisäinen tila** -asetuksena on **aloitettu**ja tieto kuplassa **ei voi lähettää vastaanottajille**.</span><span class="sxs-lookup"><span data-stu-id="6f315-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="6f315-111">Voit kiertää tämän ongelman määrittämällä työn kulun lähettämään Sähkö posti viestejä ylittämättä [Exchange Online-lähettäjän rajoituksia](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="6f315-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="6f315-112">Voit esimerkiksi käyttää keskeytystä työn kulussa, lähettää sähkö posti viestin Microsoft 365-ryhmään, jakeluun tai sähkö posti käyttöön, jossa on käytössä käyttö oikeus ryhmä, tai lähettää viestiä enintään 200 vastaanottajalla kerrallaan.</span><span class="sxs-lookup"><span data-stu-id="6f315-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="6f315-113">Lisä tietoja on seuraavassa [artikkelissa](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="6f315-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="6f315-114">Aiheeseen liittyvät artikkelit</span><span class="sxs-lookup"><span data-stu-id="6f315-114">Related topics</span></span>
- [<span data-ttu-id="6f315-115">Työn kulun luominen</span><span class="sxs-lookup"><span data-stu-id="6f315-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="6f315-116">SharePoint ja Flow</span><span class="sxs-lookup"><span data-stu-id="6f315-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 