---
title: Päivyrien hallinta
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004299"
- "7677"
ms.openlocfilehash: 2fcd0f386d2da8cad19fcc9872482bb75fe00dd2
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524631"
---
# <a name="manage-journaling"></a><span data-ttu-id="55617-102">Päivyrien hallinta</span><span class="sxs-lookup"><span data-stu-id="55617-102">Manage journaling</span></span>

<span data-ttu-id="55617-103">Kirjaaminen voi auttaa organisaatiotasi vastaamaan lakisääteisten, lakisääteisten ja organisaation vaatimustenmukaisuusvaatimuksiin kirjaamalla saapuvan ja lähtevän sähköpostiviestin.</span><span class="sxs-lookup"><span data-stu-id="55617-103">Journaling can help your organization respond to legal, regulatory, and organizational compliance requirements by recording inbound and outbound email communications.</span></span> <span data-ttu-id="55617-104">Muista:</span><span class="sxs-lookup"><span data-stu-id="55617-104">Keep in mind:</span></span>

* <span data-ttu-id="55617-105">Sinulla on oltava organisaation [hallinnan ja](https://go.microsoft.com/fwlink/?linkid=2115259) [tietueiden hallinnan](https://go.microsoft.com/fwlink/?linkid=2115469) käyttöoikeudet, ennen kuin voit hallita päivyriä.</span><span class="sxs-lookup"><span data-stu-id="55617-105">You need to have [Organization Management](https://go.microsoft.com/fwlink/?linkid=2115259) and [Records Management](https://go.microsoft.com/fwlink/?linkid=2115469) permissions before you can manage journaling.</span></span>
* <span data-ttu-id="55617-106">Sinulla on oltava päivyripostilaatikko ja (valinnaisesti) vaihtoehtoinen päivyripostilaatikko määritettynä.</span><span class="sxs-lookup"><span data-stu-id="55617-106">You need to have a journal mailbox and (optionally) an alternate journaling mailbox configured.</span></span> <span data-ttu-id="55617-107">Lisätietoja on ohjeaiheessa [Päivyrien määrittäminen Exchange Onlinessa.](https://go.microsoft.com/fwlink/?linkid=2115260)</span><span class="sxs-lookup"><span data-stu-id="55617-107">To learn more, see [Configure Journaling in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2115260).</span></span>
* <span data-ttu-id="55617-108">Exchange Onlinessa voit luoda vain päivyrisääntöjä.</span><span class="sxs-lookup"><span data-stu-id="55617-108">In Exchange Online, there's a limit to the number of journal rules that you can create.</span></span> <span data-ttu-id="55617-109">Lisätietoja on [päiväkirjan, liikenteen ja Saapuneet-kansion säännön rajoissa.](https://go.microsoft.com/fwlink/?linkid=2115261)</span><span class="sxs-lookup"><span data-stu-id="55617-109">For details, see [Journal, transport, and inbox rule limits](https://go.microsoft.com/fwlink/?linkid=2115261).</span></span>
* <span data-ttu-id="55617-110">Exchange Online ei tue päivyriraporttien toimittamista Exchange Online -postilaatikkoon.</span><span class="sxs-lookup"><span data-stu-id="55617-110">Exchange Online doesn't support delivering journal reports to an Exchange Online mailbox.</span></span> <span data-ttu-id="55617-111">Sinun on määritettävä paikallisen arkistointijärjestelmän tai kolmannen osapuolen arkistointipalvelun sähköpostiosoite päivyripostilaatikoksi.</span><span class="sxs-lookup"><span data-stu-id="55617-111">You must specify the email address of an on-premises archiving system or a third-party archiving service as the journaling mailbox.</span></span>
