---
title: SharePoint Onlinen käytön aloittaminen
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 5e61491b626bfe75fd26a15ee54be82d9efa19a7
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/15/2019
ms.locfileid: "37766888"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="45d43-102">Työn kulut SharePointissa</span><span class="sxs-lookup"><span data-stu-id="45d43-102">Workflows in SharePoint</span></span>

<span data-ttu-id="45d43-103">Jos SharePoint-työn kulut eivät lähetä sähkö posteja, organisaatiosi on saattanut kohdata Exchange Online-lähettäjän rajoitukset.</span><span class="sxs-lookup"><span data-stu-id="45d43-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="45d43-104">Työn kulku on keskeytetty-virhe sanoma saattaa ilmetä, jos sinulla on jokin seuraavista kohteista:</span><span class="sxs-lookup"><span data-stu-id="45d43-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="45d43-105">Sinulla on SharePoint Onlinen työn kulku, joka käyttää SharePoint 2010-tai SharePoint 2013-työn kulku ympäristön tyyppiä.</span><span class="sxs-lookup"><span data-stu-id="45d43-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="45d43-106">Työn kulku on määritetty lähettämään mukautettu Sähkö posti viesti yli 200 käyttäjälle kerrallaan, yli 10 000 vastaanottajaa päivässä tai yli 30 viestiä minuutissa.</span><span class="sxs-lookup"><span data-stu-id="45d43-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="45d43-107">Kun suoritat työn kulun, sähkö posti viestiä ei lähetetä ja huomaat virhe sanoman, sisäinen tila on asetettu keskeytettäväksi tai vastaanottaja ei voi lähettää vastaanottajalle.</span><span class="sxs-lookup"><span data-stu-id="45d43-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="45d43-108">Katso lisä tietoja seuraavasta [artikkelista](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span><span class="sxs-lookup"><span data-stu-id="45d43-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

