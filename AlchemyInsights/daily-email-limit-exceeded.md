---
title: Päivittäinen sähköpostiraja ylittyi. Työnkulku on keskeytetty.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 701c4aef6bfc0c4a2c4570f6dd16dbe4f99efc44
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580330"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="ae961-103">Päivittäinen sähköpostin rajoitus ylitetty.</span><span class="sxs-lookup"><span data-stu-id="ae961-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="ae961-104">Työnkulku on keskeytetty.</span><span class="sxs-lookup"><span data-stu-id="ae961-104">Workflow is suspended.</span></span>

<span data-ttu-id="ae961-105">Tämä virhe voidaan saada seuraavissa tilanteissa:</span><span class="sxs-lookup"><span data-stu-id="ae961-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="ae961-106">SharePoint Onlinessa on työnkulku, joka käyttää SharePoint 2010: n tai SharePoint 2013:n työnkulkuympäristötyyppiä.</span><span class="sxs-lookup"><span data-stu-id="ae961-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="ae961-107">Työnkulku on määritetty lähettämään mukautettu sähköpostiviesti yli 200 käyttäjälle kerrallaan, yli 10 000 vastaanottajaa päivässä tai yli 30 viestiä minuutissa.</span><span class="sxs-lookup"><span data-stu-id="ae961-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="ae961-108">Kun suoritat työnkulun, sähköpostiviestiä ei lähetetä, ja huomaat seuraavan toiminnan:</span><span class="sxs-lookup"><span data-stu-id="ae961-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="ae961-109">Jos työnkulku käyttää SharePoint 2013 -ympäristötyyppiä, siirry **Työnkulun tila -sivulle.**</span><span class="sxs-lookup"><span data-stu-id="ae961-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="ae961-110">Työnkulun tila -sivulla **Sisäinen tila** -asetuksena on **Aloitettu**ja tietoselitteen näytössä Ei voi **lähettää vastaanottajalle**.</span><span class="sxs-lookup"><span data-stu-id="ae961-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="ae961-111">Voit kiertää tämän ongelman määrittämällä työnkulun lähettämään sähköpostiviestejä ylittämättä [Exchange Onlinen lähettäjän rajoituksia](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="ae961-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="ae961-112">Käytä esimerkiksi työnkulun taukoa, lähetä sähköposti Microsoft 365 -ryhmään, jakeluryhmään tai sähköpostia käyttävään suojausryhmään tai lähetä viesti alle 200 vastaanottajalle kerrallaan.</span><span class="sxs-lookup"><span data-stu-id="ae961-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="ae961-113">Lisätietoja on seuraavassa [artikkelissa](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="ae961-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="ae961-114">Aiheeseen liittyvät artikkelit</span><span class="sxs-lookup"><span data-stu-id="ae961-114">Related topics</span></span>
- [<span data-ttu-id="ae961-115">Luo työnkulku</span><span class="sxs-lookup"><span data-stu-id="ae961-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="ae961-116">SharePoint ja Työnkulku</span><span class="sxs-lookup"><span data-stu-id="ae961-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 