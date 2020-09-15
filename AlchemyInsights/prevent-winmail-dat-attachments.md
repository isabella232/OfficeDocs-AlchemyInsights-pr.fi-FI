---
title: 2589 auttaa estämään Winmail. dat-liitteitä organisaatiosi Sähkö posti viesteissä
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2589
ms.assetid: ''
ms.openlocfilehash: f67c4146af419a590651c8e0673fd59fabd7eae7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47693732"
---
# <a name="help-prevent-winmaildat-attachments-in-email-messages-from-your-organization"></a><span data-ttu-id="f5967-102">Organisaation Sähkö posti viestien Winmail. dat-liitteiden estäminen</span><span class="sxs-lookup"><span data-stu-id="f5967-102">Help prevent Winmail.dat attachments in email messages from your organization</span></span>

<span data-ttu-id="f5967-103">Kun olet järjestelmänvalvoja, kokeile seuraavia ohjeita:</span><span class="sxs-lookup"><span data-stu-id="f5967-103">As an admin, try these steps:</span></span>

1. <span data-ttu-id="f5967-104">Avaa [Exchange-hallinta keskus](https://outlook.office365.com/ecp/).</span><span class="sxs-lookup"><span data-stu-id="f5967-104">Open the [Exchange admin center](https://outlook.office365.com/ecp/).</span></span>

2. <span data-ttu-id="f5967-105">Siirry **sähkö postin kulun**  >  **etätoimialueisiin**.</span><span class="sxs-lookup"><span data-stu-id="f5967-105">Go to **Mail flow** > **Remote domains**.</span></span>

3. <span data-ttu-id="f5967-106">Valitse oletusarvoinen etätoimialue nimeltä **oletus**ja valitse sitten **Muokkaa**.</span><span class="sxs-lookup"><span data-stu-id="f5967-106">Select the default remote domain named **Default**, and then click **Edit**.</span></span>

4. <span data-ttu-id="f5967-107">Valitse **Käytä RTF-muotoista tekstiä-** osiossa **ei koskaan**.</span><span class="sxs-lookup"><span data-stu-id="f5967-107">In the **Use Rich-text format** section, select **Never**.</span></span>

<span data-ttu-id="f5967-108">Lisä tietoja on kohdassa [etätoimialueiden viesti muodon määrittäminen](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format).</span><span class="sxs-lookup"><span data-stu-id="f5967-108">For more information, see [Specify the message format for remote domains](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format).</span></span>
