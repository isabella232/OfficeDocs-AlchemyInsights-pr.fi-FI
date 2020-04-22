---
title: Outlook Desktopin sähköpostiviestin peruuttaminen tai korvaaminen
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: d64332778f9132aff6a9660bb0d522f4e16b753c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687507"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="27fe0-102">Outlook-sähköpostiviestin peruuttaminen tai korvaaminen</span><span class="sxs-lookup"><span data-stu-id="27fe0-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="27fe0-103">Järjestelmänvalvojana voit **palauttaa viestit PowerShelliä käyttävien käyttäjien puolesta.**</span><span class="sxs-lookup"><span data-stu-id="27fe0-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="27fe0-104">Et voi palauttaa viestejä hallintakeskuksesta.</span><span class="sxs-lookup"><span data-stu-id="27fe0-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="27fe0-105">Voit **vain muistaa viestejä, jotka lähetetään organisaatiosi henkilöille.**</span><span class="sxs-lookup"><span data-stu-id="27fe0-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="27fe0-106">Jos viesti on esimerkiksi lähetetty Gmail-osoitteeseen, et voi muistaa sitä.</span><span class="sxs-lookup"><span data-stu-id="27fe0-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="27fe0-107">Voit **vain palauttaa Outlook 2016:sta lähetetyt viestit tietokoneeseen**.</span><span class="sxs-lookup"><span data-stu-id="27fe0-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="27fe0-108">Jos käyttäjä lähettää viestin Outlook for Macin tai Outlookin verkkoversiossa, et voi muistaa sitä.</span><span class="sxs-lookup"><span data-stu-id="27fe0-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="27fe0-109">Sähköpostiviestin peruuttaminen tai korvaaminen:</span><span class="sxs-lookup"><span data-stu-id="27fe0-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="27fe0-110">Valitse Outlook-ikkunan vasemmalla puolella olevasta kansioruudusta Lähetetyt-kansio.</span><span class="sxs-lookup"><span data-stu-id="27fe0-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="27fe0-111">Avaa se kaksoisnapsauttamalla viestiä, jonka haluat palauttaa.</span><span class="sxs-lookup"><span data-stu-id="27fe0-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="27fe0-112">Valitse **Viesti-välilehti** ja valitse sitten **Toiminnot, jotka** > **poistavat tämän viestin**.</span><span class="sxs-lookup"><span data-stu-id="27fe0-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="27fe0-113">Valitse **Poista tämän viestin lukemattomat kopiot** tai Poista **lukemattomat kopiot ja korvaa se uudella viestillä**ja valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="27fe0-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="27fe0-114">Jos lähetät korvaavan viestin, kirjoita viesti ja valitse sitten **Lähetä**.</span><span class="sxs-lookup"><span data-stu-id="27fe0-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="27fe0-115">Viestin peruuttaminen riippuu vastaanottajan outlook-asetuksista.</span><span class="sxs-lookup"><span data-stu-id="27fe0-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="27fe0-116">Ohjeet palautuksen tarkistamiseen ovat [tässä artikkelissa](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="27fe0-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="27fe0-117">Sähköpostiviestien etsiminen ja poistaminen organisaatiossa</span><span class="sxs-lookup"><span data-stu-id="27fe0-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="27fe0-118">Jos et ole yleinen järjestelmänvalvoja, tilisi on lisättävä eDiscovery Manager -rooliin tai Yhteensopivuushaun hallintarooliin viestien etsimistä varten.</span><span class="sxs-lookup"><span data-stu-id="27fe0-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="27fe0-119">Jos haluat poistaa viestejä, sinun on liityttävä Organisaation hallinta -rooliryhmään tai Haku- ja Tyhjennyshallinta-rooliin.</span><span class="sxs-lookup"><span data-stu-id="27fe0-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="27fe0-120">Näiden roolien käyttöoikeudet määritetään [Suojaus- ja yhteensopivuuskeskuksessa](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="27fe0-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="27fe0-121">[Luo sisältöhaku,](https://docs.microsoft.com/office365/securitycompliance/content-search) jotta voit etsiä poistettavan viestin.</span><span class="sxs-lookup"><span data-stu-id="27fe0-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="27fe0-122">[Muodosta yhteys Suojaus- ja Yhteensopivuuskeskus PowerShelliin](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="27fe0-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="27fe0-123">Jos käytät monivaiheista todennusta, katso [yhteyden muodostaminen Microsoft 365 :n suojaus- ja Yhteensopivuuskeskus PowerShelliin monivaiheisen todennuksen avulla](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="27fe0-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>