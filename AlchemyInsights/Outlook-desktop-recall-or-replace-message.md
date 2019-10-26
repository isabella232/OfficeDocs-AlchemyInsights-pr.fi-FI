---
title: Outlook Desktop muistaa tai korvata Sähkö posti viestin
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/25/2019
ms.locfileid: "36496108"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="ef700-102">Outlook-Sähkö posti viestin peruuttaminen tai korvaaminen</span><span class="sxs-lookup"><span data-stu-id="ef700-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="ef700-103">Järjestelmänvalvojana voit **peruuttaa viestit käyttäjien puolesta PowerShellin avulla**.</span><span class="sxs-lookup"><span data-stu-id="ef700-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="ef700-104">Et voi peruuttaa viestejä hallinta keskuksesta.</span><span class="sxs-lookup"><span data-stu-id="ef700-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="ef700-105">Voit **peruuttaa vain organisaatiosi henkilöille lähetetyt viestit**.</span><span class="sxs-lookup"><span data-stu-id="ef700-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="ef700-106">Jos viesti lähetettiin esimerkiksi Gmail-osoitteeseen, et voi muistaa sitä.</span><span class="sxs-lookup"><span data-stu-id="ef700-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="ef700-107">Voit **peruuttaa vain Outlook 2016-tieto koneella lähetetyt viestit**.</span><span class="sxs-lookup"><span data-stu-id="ef700-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="ef700-108">Jos käyttäjä lähettää viestin Outlookin Mac-tai Outlook-tieto koneella, et voi muistaa sitä.</span><span class="sxs-lookup"><span data-stu-id="ef700-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="ef700-109">Sähkö posti viestin peruuttaminen tai korvaaminen:</span><span class="sxs-lookup"><span data-stu-id="ef700-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="ef700-110">Valitse Outlook-ikkunan vasemmalla puolella olevasta kansio ruudusta Lähetetyt-kansio.</span><span class="sxs-lookup"><span data-stu-id="ef700-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="ef700-111">Kaksoisnapsauta viestiä, jonka haluat peruuttaa, ja avaa se.</span><span class="sxs-lookup"><span data-stu-id="ef700-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="ef700-112">Valitse **viesti** -väli lehti ja valitse sitten **toiminnot** > **Muista tämä viesti**.</span><span class="sxs-lookup"><span data-stu-id="ef700-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="ef700-113">Valitse **Poista tämän viestin lukemattomat kopiot** tai **Poista lukemattomat kopiot ja korvaa ne uudella viestillä**ja valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="ef700-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="ef700-114">Jos lähetät korvaavan viestin, kirjoita viesti ja valitse sitten **Lähetä**.</span><span class="sxs-lookup"><span data-stu-id="ef700-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="ef700-115">Viestin muistamisen onnistuminen tai epäonnistuminen riippuu vastaanottajan asetuksista Outlookissa.</span><span class="sxs-lookup"><span data-stu-id="ef700-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="ef700-116">Lisä ohjeita takaisinkutsun tarkastamisen osalta [on tässä artikkelissa](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="ef700-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="ef700-117">Etsi ja poista Sähkö posti viestejä organisaatiossasi</span><span class="sxs-lookup"><span data-stu-id="ef700-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="ef700-118">Jos et ole yleinen järjestelmänvalvoja, sinun tilisi on lisättävä eDiscovery Managerin rooliin tai yhteensopivuuden haun hallinta rooliin, jotta voit etsiä viestejä.</span><span class="sxs-lookup"><span data-stu-id="ef700-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="ef700-119">Jos haluat poistaa viestejä, sinun on liityttävä organisaation hallinta-rooli ryhmään tai haun ja Tyhjennen hallinnan rooliin.</span><span class="sxs-lookup"><span data-stu-id="ef700-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="ef700-120">Näiden roolien käyttö oikeudet määritetään [Suojaus-ja yhteensopivuus keskuksessa](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="ef700-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="ef700-121">Etsi poistettava viesti [luomalla sisältö haku](https://docs.microsoft.com/office365/securitycompliance/content-search) .</span><span class="sxs-lookup"><span data-stu-id="ef700-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="ef700-122">[Muodosta yhteys tieto turva-ja yhteensopivuus keskukseen PowerShelliin](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="ef700-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="ef700-123">Jos käytät monivaiheista todennusta, katso [yhteyden muodostaminen Office 365 Security and Compliance Center PowerShelliin monimivaiheisen todennuksen avulla](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="ef700-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>