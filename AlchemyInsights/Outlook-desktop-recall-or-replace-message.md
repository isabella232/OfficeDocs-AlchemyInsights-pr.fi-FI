---
title: Työpöydän Outlook-peruutus- tai korvaa sähköpostiviestin
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: aced684777ef82860b969aea8825699b78b04c5a
ms.sourcegitcommit: aad9f863bc9fd7d5522c480bd1a7d15f3a80ff4f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/15/2019
ms.locfileid: "30657041"
---
# <a name="recall-or-replace-an-email-message"></a><span data-ttu-id="7e7ae-102">Peruuttaa tai korvata sähköpostiviestin</span><span class="sxs-lookup"><span data-stu-id="7e7ae-102">Recall or replace an email message</span></span>

- <span data-ttu-id="7e7ae-103">Voit järjestelmänvalvojana, **peruutus viestien PowerShell avulla käyttäjien puolesta**.</span><span class="sxs-lookup"><span data-stu-id="7e7ae-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="7e7ae-104">Ei voi peruuttaa viestien hallintakeskukseen.</span><span class="sxs-lookup"><span data-stu-id="7e7ae-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="7e7ae-105">Voit **vain palauttaa viestit, jotka lähetetään organisaation henkilöt**.</span><span class="sxs-lookup"><span data-stu-id="7e7ae-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="7e7ae-106">Jos viesti lähetettiin Gmail-osoite, esimerkiksi et pysty peruuttamaan sen.</span><span class="sxs-lookup"><span data-stu-id="7e7ae-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="7e7ae-107">Voit **vain peruutus kulku Outlook-2016, PC: ssä**.</span><span class="sxs-lookup"><span data-stu-id="7e7ae-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="7e7ae-108">Jos käyttäjä lähettää viestin käyttäen Mac Outlook tai Outlook Web, se ei voi peruuttaa.</span><span class="sxs-lookup"><span data-stu-id="7e7ae-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="7e7ae-109">Voit peruuttaa tai korvata sähköpostiviestin:</span><span class="sxs-lookup"><span data-stu-id="7e7ae-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="7e7ae-110">Valitse kansioruudusta Outlook-ikkunan vasemmassa reunassa Lähetetyt-kansioon.</span><span class="sxs-lookup"><span data-stu-id="7e7ae-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="7e7ae-111">Kaksoisnapsauta viestiä, jonka haluat peruuttaa, voit avata sen.</span><span class="sxs-lookup"><span data-stu-id="7e7ae-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="7e7ae-112">Valitse **sanoma** -välilehti ja valitse sitten **Toiminnot** > **Peruuta viesti**.</span><span class="sxs-lookup"><span data-stu-id="7e7ae-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="7e7ae-113">Valitse **poistaa viestin lukemattomat kopiot** tai **poistaa viestin lukemattomat kopiot ja korvata uudella viestillä**ja valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="7e7ae-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="7e7ae-114">Jos lähetät korvaavan viestin, viestin, ja valitse sitten **Lähetä**.</span><span class="sxs-lookup"><span data-stu-id="7e7ae-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="7e7ae-115">Onnistuminen tai epäonnistuminen on viesti on riippuvainen vastaanottajan Outlook-asetuksista.</span><span class="sxs-lookup"><span data-stu-id="7e7ae-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="7e7ae-116">Lisätietoja tarkistamisesta peruutus on [Tässä artikkelissa](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="7e7ae-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="7e7ae-117">Etsi ja poista viestejä organisaation</span><span class="sxs-lookup"><span data-stu-id="7e7ae-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="7e7ae-118">Jos et ole yleinen järjestelmänvalvoja, tili on lisättävä eDiscovery hallinnan rooli tai yhteensopivuuden haun hallinnan roolin voit hakea viestejä.</span><span class="sxs-lookup"><span data-stu-id="7e7ae-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="7e7ae-119">Jos haluat poistaa viestejä, tarvitset liittyä organisaation hallinta-rooliryhmän tai etsintä- ja poisto-hallinnan roolin.</span><span class="sxs-lookup"><span data-stu-id="7e7ae-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="7e7ae-120">Näiden roolien käyttöoikeuksista on liitetty [center tietoturvan ja määritystenmukaisuuden suhteen](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="7e7ae-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="7e7ae-121">Voit etsiä poistettavan viestin [luominen on etsiä](https://docs.microsoft.com/office365/securitycompliance/content-search) .</span><span class="sxs-lookup"><span data-stu-id="7e7ae-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="7e7ae-122">[Security and Compliance Centeriin PowerShell muodostaa](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="7e7ae-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="7e7ae-123">Jos käytät monitasoisen todennuksen, katso [yhteyden Office 365: n tietoturvan ja yhteensopivuuden Center PowerShell monitasoisen todennuksen](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="7e7ae-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>