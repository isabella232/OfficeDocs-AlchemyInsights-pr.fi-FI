---
title: Outlookin Työpöytä version peruuttaminen tai sähkö posti viestin korvaaminen
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663987"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="10e12-102">Outlook-Sähkö posti viestin peruuttaminen tai korvaaminen</span><span class="sxs-lookup"><span data-stu-id="10e12-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="10e12-103">Järjestelmänvalvojana voit **peruuttaa viestejä käyttäjien puolesta PowerShellin avulla**.</span><span class="sxs-lookup"><span data-stu-id="10e12-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="10e12-104">Et voi peruuttaa viestejä hallinta keskuksesta.</span><span class="sxs-lookup"><span data-stu-id="10e12-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="10e12-105">Voit **peruuttaa vain organisaation henkilöille lähetetyt viestit**.</span><span class="sxs-lookup"><span data-stu-id="10e12-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="10e12-106">Jos viesti on lähetetty Gmail-osoitteeseen, et voi esimerkiksi peruuttaa sitä.</span><span class="sxs-lookup"><span data-stu-id="10e12-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="10e12-107">Voit **vain peruuttaa viestit, jotka on lähetetty Outlook 2016-tieto koneesta**.</span><span class="sxs-lookup"><span data-stu-id="10e12-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="10e12-108">Jos käyttäjä lähettää viestin käyttämällä Outlook for Macia tai Outlookin verkko versiota, et voi peruuttaa sitä.</span><span class="sxs-lookup"><span data-stu-id="10e12-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="10e12-109">Sähkö posti viestin peruuttaminen tai korvaaminen:</span><span class="sxs-lookup"><span data-stu-id="10e12-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="10e12-110">Valitse Outlook-ikkunan vasemmalla puolella olevassa kansio ruudussa Lähetetyt-kansio.</span><span class="sxs-lookup"><span data-stu-id="10e12-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="10e12-111">Avaa viesti, jonka haluat peruuttaa, kaksoisnapsauttamalla sitä.</span><span class="sxs-lookup"><span data-stu-id="10e12-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="10e12-112">Valitse **viesti** -väli lehti ja valitse sitten **toiminnot**, jotka  >  **palauttavat tämän viestin**.</span><span class="sxs-lookup"><span data-stu-id="10e12-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="10e12-113">Valitse **Poista tämän viestin lukemattomat kopiot** tai **Poista lukemattomat kopiot ja vaihda uuteen viestiin**ja valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="10e12-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="10e12-114">Jos lähetät korvaavan viestin, kirjoita viesti ja valitse sitten **Lähetä**.</span><span class="sxs-lookup"><span data-stu-id="10e12-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="10e12-115">Viestin peruuttamisen onnistuminen tai epäonnistuminen määräytyy sen mukaan, mitä vastaanottajia koskevat asetukset ovat Outlookissa.</span><span class="sxs-lookup"><span data-stu-id="10e12-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="10e12-116">Jos haluat tarkistaa peruutuksen, Lue [Tämä artikkeli](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="10e12-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="10e12-117">Sähkö posti viestien etsiminen ja poistaminen organisaatiossa</span><span class="sxs-lookup"><span data-stu-id="10e12-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="10e12-118">Jos et ole yleinen järjestelmänvalvoja, tili on lisättävä eDiscoveryn hallinta rooliin tai yhteensopivuuden haun hallinta rooliin, jotta voit hakea viestejä.</span><span class="sxs-lookup"><span data-stu-id="10e12-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="10e12-119">Jos haluat poistaa viestejä, sinun on liitytä organisaation hallinta-rooli ryhmään tai Hae ja poista hallinta-rooliin.</span><span class="sxs-lookup"><span data-stu-id="10e12-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="10e12-120">Näiden roolien käyttö oikeudet määritetään [tieto turva-ja yhteensopivuus keskuksessa](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="10e12-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="10e12-121">[Luo sisältö haku](https://docs.microsoft.com/microsoft-365/compliance/content-search) , jos haluat etsiä poistettavan viestin.</span><span class="sxs-lookup"><span data-stu-id="10e12-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="10e12-122">[Muodosta yhteys tieto turva-ja yhteensopivuus keskuksen PowerShellin avulla](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="10e12-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="10e12-123">Jos käytät monimenetelmäistä todennusta, Katso lisä tietoja artikkelista [yhteyden muodostaminen Microsoft 365-tieto turva-ja yhteensopivuus keskuksen PowerShellin avulla monimenetelmäinen todentaminen-toiminnolla](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="10e12-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>