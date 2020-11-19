---
title: Sähkö posti viestin peruuttaminen tai korvaaminen
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353503"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="a432d-102">Sähkö posti viestin peruuttaminen tai korvaaminen Microsoft 365-sovelluksessa</span><span class="sxs-lookup"><span data-stu-id="a432d-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="a432d-103">Voit **peruuttaa vain organisaation henkilöille lähetetyt viestit**.</span><span class="sxs-lookup"><span data-stu-id="a432d-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="a432d-104">Jos viesti on esimerkiksi lähetetty Gmail-osoitteeseen, et voi peruuttaa sitä.</span><span class="sxs-lookup"><span data-stu-id="a432d-104">For example, if the message was sent to a Gmail address, you can't recall it.</span></span>
- <span data-ttu-id="a432d-105">Voit **vain peruuttaa viestit, jotka on lähetetty Outlookista PC-tieto koneelle**.</span><span class="sxs-lookup"><span data-stu-id="a432d-105">You can **only recall messages sent from Outlook for the PC**.</span></span> <span data-ttu-id="a432d-106">Jos käyttäjä lähettää viestin käyttämällä Outlook for Macia tai Outlookin verkko versiota, et voi peruuttaa sitä.</span><span class="sxs-lookup"><span data-stu-id="a432d-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="a432d-107">Vuokra ajan järjestelmänvalvojana voit **peruuttaa viestit käyttäjien puolesta PowerShellin avulla** (lisä tietoja on artikkeleissa [Sähkö posti viestien etsiminen ja poistaminen](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span><span class="sxs-lookup"><span data-stu-id="a432d-107">As a tenant administrator, you can **recall messages on behalf of users by using PowerShell** (For more information, see: [Search for and delete email messages](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span></span>
- <span data-ttu-id="a432d-108">Et voi peruuttaa viestejä hallinta keskuksesta.</span><span class="sxs-lookup"><span data-stu-id="a432d-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="a432d-109">Lisä tietoja on kohdassa Sähkö posti viestien etsiminen ja poistaminen organisaatiossa.</span><span class="sxs-lookup"><span data-stu-id="a432d-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="a432d-110">**Lähetetyn Sähkö posti viestin peruuttaminen tai korvaaminen**</span><span class="sxs-lookup"><span data-stu-id="a432d-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="a432d-111">Valitse Outlook-ikkunan vasemmalla puolella olevassa kansio ruudussa Lähetetyt-kansio.</span><span class="sxs-lookup"><span data-stu-id="a432d-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="a432d-112">Avaa viesti, jonka haluat peruuttaa.</span><span class="sxs-lookup"><span data-stu-id="a432d-112">Open the message that you want to recall.</span></span> <span data-ttu-id="a432d-113">Sinun on avattava viesti kaksoisnapsauttamalla.</span><span class="sxs-lookup"><span data-stu-id="a432d-113">You must double-click to open the message.</span></span> <span data-ttu-id="a432d-114">Kun valitset viestin niin, että se näkyy luku ruudussa, et voi peruuttaa viestiä.</span><span class="sxs-lookup"><span data-stu-id="a432d-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="a432d-115">Valitse viesti-väli lehdessä **toiminnot**, jotka  >  **palauttavat tämän viestin**.</span><span class="sxs-lookup"><span data-stu-id="a432d-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="a432d-116">Valitse **Poista viestin lukemattomat kopiot** tai **Poista lukemattomat kopiot ja vaihda uudella viestillä ja** valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="a432d-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="a432d-117">Jos lähetät korvaavan viestin, kirjoita viesti ja valitse sitten **Lähetä**.</span><span class="sxs-lookup"><span data-stu-id="a432d-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="a432d-118">Viestin peruuttamisen onnistuminen tai epäonnistuminen määräytyy Outlookin edunsaajien asetusten mukaan.</span><span class="sxs-lookup"><span data-stu-id="a432d-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="a432d-119">Lisä tietoja, kuten peruutuksen tarkistaminen, on kohdassa [lähetetyn Sähkö posti viestin peruuttaminen tai korvaaminen](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="a432d-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="a432d-120">Jos haluat **_etsiä ja poistaa organisaatiosi Sähkö posti viestejä_**, se on helpointa, jos olet yleinen järjestelmänvalvoja. Jos et ole yleinen järjestelmänvalvoja, tili on lisättävä eDiscoveryn hallinnan rooli ryhmään tai yhteensopivuuden haun hallinta rooliin.</span><span class="sxs-lookup"><span data-stu-id="a432d-120">**_To search for and delete email messages in your organization_**, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="a432d-121">Jos haluat poistaa viestejä, sinun on liitytä organisaation hallinta-rooli ryhmään tai Hae ja poista hallinta-rooliin.</span><span class="sxs-lookup"><span data-stu-id="a432d-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="a432d-122">Näiden roolien käyttö oikeudet määritetään [suojaus & yhteensopivuus keskuksessa](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="a432d-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="a432d-123">[Luo sisältö haku](https://docs.microsoft.com/microsoft-365/compliance/content-search) , jos haluat etsiä poistettavan viestin.</span><span class="sxs-lookup"><span data-stu-id="a432d-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="a432d-124">[Muodosta yhteys tieto turva & Compliance Center PowerShellin avulla](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="a432d-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span>

<span data-ttu-id="a432d-125">Jos käytössäsi on MFA (monimenetelmäinen todentaminen), Katso lisä tietoja artikkelista [yhteyden muodostaminen Microsoft 365-tieto turva & yhteensopivuus keskuksen PowerShell monimenetelmäisen todentamisen avulla](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="a432d-125">If you're using MFA (multi-factor authentication), see [Connect to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span></span>
