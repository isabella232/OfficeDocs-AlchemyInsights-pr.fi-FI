---
title: 2589 estää Winmail.dat-liitteitä sähköpostiviestejä-organisaatiolta
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2589
ms.assetid: ''
ms.openlocfilehash: 41ab3f22499994cda5883834ff54e5767c69265b
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391243"
---
# <a name="help-prevent-winmaildat-attachments-in-email-messages-from-your-organization"></a><span data-ttu-id="60051-102">Winmail.dat-liitteitä organisaatiolta sähköposti viestien estäminen</span><span class="sxs-lookup"><span data-stu-id="60051-102">Help prevent Winmail.dat attachments in email messages from your organization</span></span>

<span data-ttu-id="60051-103">Järjestelmänvalvojana toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="60051-103">As an admin, try these steps:</span></span>

1. <span data-ttu-id="60051-104">Avaa [Exchange-hallintakeskukseen](https://outlook.office365.com/ecp/).</span><span class="sxs-lookup"><span data-stu-id="60051-104">Open the [Exchange admin center](https://outlook.office365.com/ecp/).</span></span>

2. <span data-ttu-id="60051-105">Siirry **postin kulku** > **Remote toimialueet**.</span><span class="sxs-lookup"><span data-stu-id="60051-105">Go to **Mail flow** > **Remote domains**.</span></span>

3. <span data-ttu-id="60051-106">Valitse oletus etätoimialueen nimeltä **Oletus**ja valitse sitten **Muokkaa**.</span><span class="sxs-lookup"><span data-stu-id="60051-106">Select the default remote domain named **Default**, and then click **Edit**.</span></span>

4. <span data-ttu-id="60051-107">**Käytä RTF - muotoilu** -osan Valitse **ei koskaan**.</span><span class="sxs-lookup"><span data-stu-id="60051-107">In the **Use Rich-text format** section, select **Never**.</span></span>

<span data-ttu-id="60051-108">Lisätietoja [Määritä etä toimialueiden muotoa](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format).</span><span class="sxs-lookup"><span data-stu-id="60051-108">For more information, see [Specify the message format for remote domains](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format).</span></span>
