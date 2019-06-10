---
title: Aloittaminen SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: afb1ef115d364ee3e2cf09ea850adb57ad1d44e6
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34770560"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="4d57e-102">SharePoint-työnkulkuja</span><span class="sxs-lookup"><span data-stu-id="4d57e-102">Workflows in SharePoint</span></span>

<span data-ttu-id="4d57e-103">SharePoint-työnkulkuja ei lähetetä sähköpostia, jos organisaation on kohdannut Exchange Onlinen lähettäjän rajat.</span><span class="sxs-lookup"><span data-stu-id="4d57e-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="4d57e-104">'Työnkulku keskeytetään ”virhesanoma voi tulla näyttöön, jos sinulla on jokin seuraavista:</span><span class="sxs-lookup"><span data-stu-id="4d57e-104">'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="4d57e-105">On työnkulun SharePoint Online, joka käyttää SharePoint 2010 tai SharePoint 2013-työnkulun ympäristötyyppi.</span><span class="sxs-lookup"><span data-stu-id="4d57e-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="4d57e-106">Jos haluat lähettää mukautetun sähköpostiviestin käyttäjille yli 200 kertaa, yli 10 000 vastaanottajaa päivässä tai yli 30 minuutissa viestit työnkulku on määritetty.</span><span class="sxs-lookup"><span data-stu-id="4d57e-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="4d57e-107">Työnkulun suoritus ei lähetetä sähköpostiviestin ja huomaat virhesanoma tulee näyttöön, kun sisäinen tilaksi määritetään Suspended tai ei voi lähettää vastaanottajalle.</span><span class="sxs-lookup"><span data-stu-id="4d57e-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="4d57e-108">Saat lisätietoja tutustu seuraavassa [artikkelissa](https://support.office.com/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US).</span><span class="sxs-lookup"><span data-stu-id="4d57e-108">For more information, please refer to the following [article](https://support.office.com/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

