---
title: Päivittäinen sähköpostiviesti raja on ylitetty. Työnkulku on pysäytetty.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: e3fbcd5bfc279847cfb39140c3689f5433b61509
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36514446"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="102fb-103">Päivittäinen email raja ylitetty.</span><span class="sxs-lookup"><span data-stu-id="102fb-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="102fb-104">Työnkulku on pysäytetty.</span><span class="sxs-lookup"><span data-stu-id="102fb-104">Workflow is suspended.</span></span>

<span data-ttu-id="102fb-105">Tämä virhe voi vastaanottaa seuraavissa tilanteissa:</span><span class="sxs-lookup"><span data-stu-id="102fb-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="102fb-106">On työnkulun SharePoint Online, joka käyttää SharePoint 2010 tai SharePoint 2013-työnkulun ympäristötyyppi.</span><span class="sxs-lookup"><span data-stu-id="102fb-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="102fb-107">Jos haluat lähettää mukautetun sähköpostiviestin käyttäjille yli 200 kertaa, yli 10 000 vastaanottajaa päivässä tai yli 30 minuutissa viestit työnkulku on määritetty.</span><span class="sxs-lookup"><span data-stu-id="102fb-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="102fb-108">Kun suoritat työnkulun, sähköpostiviestiä ei lähetetä ja huomata seuraavia ongelmia:</span><span class="sxs-lookup"><span data-stu-id="102fb-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="102fb-109">Työnkulun SharePoint-2013 ympäristö-tyyppiä käyttäen selaamalla **Työnkulun tila** -sivun.</span><span class="sxs-lookup"><span data-stu-id="102fb-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="102fb-110">Työnkulun tila-sivun **Sisäinen tila** määritetään **Aloitettu**ja näyttää tiedot ilmoitusta **ei voi lähettää vastaanottajalle**.</span><span class="sxs-lookup"><span data-stu-id="102fb-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="102fb-111">Voit kiertää tämän ongelman, Määritä työnkulun lähettämään sähköpostiviestejä [Exchange Onlinen lähettäjän rajoja](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)ylittämättä.</span><span class="sxs-lookup"><span data-stu-id="102fb-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="102fb-112">Esimerkiksi käyttää työnkulun tauon, Lähetä sähköposti Office 365-ryhmän jakeluryhmä tai suojausryhmä sähköpostin käytössä tai lähettää viestin alle 200 vastaanottajalle kerrallaan.</span><span class="sxs-lookup"><span data-stu-id="102fb-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="102fb-113">Lisätietoja on seuraavassa [artikkelissa](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="102fb-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="102fb-114">Aiheeseen liittyvät artikkelit</span><span class="sxs-lookup"><span data-stu-id="102fb-114">Related topics</span></span>
- [<span data-ttu-id="102fb-115">Luo työnkulku</span><span class="sxs-lookup"><span data-stu-id="102fb-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="102fb-116">SharePoint- ja</span><span class="sxs-lookup"><span data-stu-id="102fb-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 