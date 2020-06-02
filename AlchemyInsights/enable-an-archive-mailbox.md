---
title: Arkistopostilaatikon ottaminen käyttöön
ms.author: markjjo
author: markjjo
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "307"
- "3100008"
ms.assetid: e1a5fab7-d3a5-4d4c-8ee2-0edf4ec9b76b
ms.openlocfilehash: 2eecb51a2a6bf2e0741b7ee14dca16f8e0ad4c61
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507023"
---
# <a name="enable-an-archive-mailbox"></a><span data-ttu-id="4d282-102">Arkistopostilaatikon ottaminen käyttöön</span><span class="sxs-lookup"><span data-stu-id="4d282-102">Enable an archive mailbox</span></span>

<span data-ttu-id="4d282-103">Arkisto postilaatikot Microsoft 365 (kutsutaan myös *Online Archives* tai *In-Place Arkisto*) tarjota käyttäjille lisää sähköpostin varastointi.</span><span class="sxs-lookup"><span data-stu-id="4d282-103">Archive mailboxes in Microsoft 365 (also called *Online Archives* or *In-Place Archives*) provide users with additional email storage.</span></span> <span data-ttu-id="4d282-104">Käyttäjät voivat siirtää tai kopioida kohteita arkistopostilaatikkoonsa, ja järjestelmänvalvojat voivat luoda arkistokäytännön, joka siirtää kohteet automaattisesti arkistopostilaatikoihin.</span><span class="sxs-lookup"><span data-stu-id="4d282-104">Users can move or copy items to their archive mailbox, and admins can create an archive policy that automatically moves items to archive mailboxes.</span></span>
  
<span data-ttu-id="4d282-105">Voit luoda arkistopostilaatikon seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="4d282-105">Here's how to create an archive mailbox:</span></span>
  
1. <span data-ttu-id="4d282-106">Siirry osoitteeseen [https://protection.office.com](https://protection.office.com).</span><span class="sxs-lookup"><span data-stu-id="4d282-106">Go to [https://protection.office.com](https://protection.office.com).</span></span>

2. <span data-ttu-id="4d282-107">Kirjaudu Microsoft 365:lle järjestelmänvalvojan tililläsi.</span><span class="sxs-lookup"><span data-stu-id="4d282-107">Sign in to Microsoft 365 using your admin account.</span></span>

3. <span data-ttu-id="4d282-108">Valitse Tietoturvan yhteensopivuuskeskuksen vasemmasta ruudusta &amp; **Tietojen hallinta** \> **Arkisto**.</span><span class="sxs-lookup"><span data-stu-id="4d282-108">In the left pane of the Security &amp; Compliance Center, select **Information governance** \> **Archive**.</span></span>

4. <span data-ttu-id="4d282-109">Valitse käyttäjä, jonka arkistopostilaatikon haluat ottaa käyttöön.</span><span class="sxs-lookup"><span data-stu-id="4d282-109">Select the user whose archive mailbox you want to enable.</span></span>

5. <span data-ttu-id="4d282-110">Valitse oikeanpuoleisessa tietoruudussa **Ota käyttöön** ja ota arkistopostilaatikko käyttöön valitsemalla varoitusviestissä **Kyllä.**</span><span class="sxs-lookup"><span data-stu-id="4d282-110">In the details pane on the right, click **Enable** and then click **Yes** in the warning message to enable the archive mailbox.</span></span>

<span data-ttu-id="4d282-111">Voit myös ottaa arkistopostilaatikot käyttöön joukkoon valitsemalla useita käyttäjiä **(Vaihto-** tai Ctrl-näppäimillä) ja valitsemalla sitten **tietoruudussa Ota käyttöön.** **Ctrl**</span><span class="sxs-lookup"><span data-stu-id="4d282-111">You can also bulk-enable archive mailboxes by selecting multiple users (using the **Shift** or **Ctrl** keys) and then clicking **Enable** in the details pane.</span></span>
  
### <a name="shared-mailboxes"></a><span data-ttu-id="4d282-112">Jaetut postilaatikot</span><span class="sxs-lookup"><span data-stu-id="4d282-112">Shared mailboxes</span></span>

<span data-ttu-id="4d282-113">Jaetun postilaatikon arkiston käyttöönotto edellyttää Exchange Online -palvelupaketin 2 käyttöoikeutta tai Exchange Online -palvelupaketin 1 käyttöoikeutta, jolla on Exchange Online Archiving -käyttöoikeus.</span><span class="sxs-lookup"><span data-stu-id="4d282-113">To enable the archive for a shared mailbox, an Exchange Online Plan 2 license or an Exchange Online Plan 1 license with an Exchange Online Archiving license is required.</span></span>  

<span data-ttu-id="4d282-114">Jaetun postilaatikon arkiston ottaminen käyttöön:</span><span class="sxs-lookup"><span data-stu-id="4d282-114">To enable the archive for a shared mailbox:</span></span>

1. <span data-ttu-id="4d282-115">Siirry [Exchange-hallintakeskukseen](https://outlook.office365.com/ecp) ja kirjaudu sisään järjestelmänvalvojan tililläsi.</span><span class="sxs-lookup"><span data-stu-id="4d282-115">Go to the [Exchange admin center](https://outlook.office365.com/ecp) and sign in using your admin account.</span></span>

2. <span data-ttu-id="4d282-116">Siirry **Jaettuihin vastaanottajiin**  >  **Shared**.</span><span class="sxs-lookup"><span data-stu-id="4d282-116">Go to **Recipients** > **Shared**.</span></span>

3. <span data-ttu-id="4d282-117">Valitse jaettu postilaatikko.</span><span class="sxs-lookup"><span data-stu-id="4d282-117">Select the shared mailbox.</span></span>

4. <span data-ttu-id="4d282-118">Valitse oikealla olevan tietoruudun **In-Place Archive -kohdassa** **Ota käyttöön**ja ota arkistopostilaatikko käyttöön valitsemalla **Kyllä.**</span><span class="sxs-lookup"><span data-stu-id="4d282-118">In the details pane on the right, under **In-Place Archive**, click **Enable**, and then click **Yes** to enable the archive mailbox.</span></span>

<span data-ttu-id="4d282-119">Lisätietoja on seuraavissa artikkeleissa:</span><span class="sxs-lookup"><span data-stu-id="4d282-119">For more information, see:</span></span>
  
- [<span data-ttu-id="4d282-120">Arkistopostilaatikoiden ottaminen käyttöön</span><span class="sxs-lookup"><span data-stu-id="4d282-120">Enable archive mailboxes</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes)

- [<span data-ttu-id="4d282-121">Arkisto- ja poistokäytännön määrittäminen</span><span class="sxs-lookup"><span data-stu-id="4d282-121">Set up an archive and deletion policy</span></span>](https://docs.microsoft.com//office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes)
