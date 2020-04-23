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
ms.openlocfilehash: 5f5fea1e442b489bc81d9f6c4213e302c80f4ea7
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43788663"
---
# <a name="enable-an-archive-mailbox"></a><span data-ttu-id="35a15-102">Arkistopostilaatikon ottaminen käyttöön</span><span class="sxs-lookup"><span data-stu-id="35a15-102">Enable an archive mailbox</span></span>

<span data-ttu-id="35a15-103">Arkistopostilaatikot Microsoft 365:ssä (kutsutaan myös *online-arkistoiksi* tai *in-place-arkistoiksi)* tarjoavat käyttäjille lisää sähköpostisäilöä.</span><span class="sxs-lookup"><span data-stu-id="35a15-103">Archive mailboxes in Microsoft 365 (also called *Online Archives* or *In-Place Archives*) provide users with additional email storage.</span></span> <span data-ttu-id="35a15-104">Käyttäjät voivat siirtää tai kopioida kohteita arkistopostilaatikkoonsa, ja järjestelmänvalvojat voivat luoda arkistokäytännön, joka siirtää kohteet automaattisesti arkistopostilaatikoihin.</span><span class="sxs-lookup"><span data-stu-id="35a15-104">Users can move or copy items to their archive mailbox, and admins can create an archive policy that automatically moves items to archive mailboxes.</span></span>
  
<span data-ttu-id="35a15-105">Voit luoda arkistopostilaatikon seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="35a15-105">Here's how to create an archive mailbox:</span></span>
  
1. <span data-ttu-id="35a15-106">Siirry osoitteeseen [https://protection.office.com](https://protection.office.com).</span><span class="sxs-lookup"><span data-stu-id="35a15-106">Go to [https://protection.office.com](https://protection.office.com).</span></span>

2. <span data-ttu-id="35a15-107">Kirjaudu Microsoft 365:een järjestelmänvalvojan tililläsi.</span><span class="sxs-lookup"><span data-stu-id="35a15-107">Sign in to Microsoft 365 using your admin account.</span></span>

3. <span data-ttu-id="35a15-108">Valitse &amp; Tietoturvan yhteensopivuuskeskuksen vasemmasta ruudusta **Tietojen hallintaarkisto** \> **Archive**.</span><span class="sxs-lookup"><span data-stu-id="35a15-108">In the left pane of the Security &amp; Compliance Center, select **Information governance** \> **Archive**.</span></span>

4. <span data-ttu-id="35a15-109">Valitse käyttäjä, jonka arkistopostilaatikon haluat ottaa käyttöön.</span><span class="sxs-lookup"><span data-stu-id="35a15-109">Select the user whose archive mailbox you want to enable.</span></span>

5. <span data-ttu-id="35a15-110">Valitse oikeanpuoleisessa tietoruudussa **Ota käyttöön** ja ota arkistopostilaatikko käyttöön valitsemalla varoitussanomassa **Kyllä.**</span><span class="sxs-lookup"><span data-stu-id="35a15-110">In the details pane on the right, click **Enable** and then click **Yes** in the warning message to enable the archive mailbox.</span></span>

<span data-ttu-id="35a15-111">Voit myös ottaa arkistopostilaatikot käyttöön kerralla valitsemalla useita käyttäjiä **(vaihto-** tai Ctrl-näppäimillä) ja valitsemalla sitten tietoruudussa **Ota käyttöön.** **Ctrl**</span><span class="sxs-lookup"><span data-stu-id="35a15-111">You can also bulk-enable archive mailboxes by selecting multiple users (using the **Shift** or **Ctrl** keys) and then clicking **Enable** in the details pane.</span></span>
  
### <a name="shared-mailboxes"></a><span data-ttu-id="35a15-112">Jaetut postilaatikot</span><span class="sxs-lookup"><span data-stu-id="35a15-112">Shared mailboxes</span></span>

<span data-ttu-id="35a15-113">Jaetun postilaatikon arkiston käyttöönotto edellyttää Exchange Online -palvelupaketin 2 käyttöoikeutta tai Exchange Online -palvelupaketin 1 käyttöoikeutta Exchange Online Archiving -käyttöotolla.</span><span class="sxs-lookup"><span data-stu-id="35a15-113">To enable the archive for a shared mailbox, an Exchange Online Plan 2 license or an Exchange Online Plan 1 license with an Exchange Online Archiving license is required.</span></span>  

<span data-ttu-id="35a15-114">Jaetun postilaatikon arkiston ottaminen käyttöön:</span><span class="sxs-lookup"><span data-stu-id="35a15-114">To enable the archive for a shared mailbox:</span></span>

1. <span data-ttu-id="35a15-115">Siirry [Exchange-hallintakeskukseen](https://outlook.office365.com/ecp) ja kirjaudu sisään järjestelmänvalvojan tililläsi.</span><span class="sxs-lookup"><span data-stu-id="35a15-115">Go to the [Exchange admin center](https://outlook.office365.com/ecp) and sign in using your admin account.</span></span>

2. <span data-ttu-id="35a15-116">**Siirry** > **vastaanottajille jaettu**.</span><span class="sxs-lookup"><span data-stu-id="35a15-116">Go to **Recipients** > **Shared**.</span></span>

3. <span data-ttu-id="35a15-117">Valitse jaettu postilaatikko.</span><span class="sxs-lookup"><span data-stu-id="35a15-117">Select the shared mailbox.</span></span>

4. <span data-ttu-id="35a15-118">Valitse oikeanpuoleisen tietoruudun **In-Place Archive -kohdassa** **Ota käyttöön**ja ota arkistopostilaatikko käyttöön valitsemalla **Kyllä.**</span><span class="sxs-lookup"><span data-stu-id="35a15-118">In the details pane on the right, under **In-Place Archive**, click **Enable**, and then click **Yes** to enable the archive mailbox.</span></span>

<span data-ttu-id="35a15-119">Lisätietoja on seuraavissa artikkeleissa:</span><span class="sxs-lookup"><span data-stu-id="35a15-119">For more information, see:</span></span>
  
- [<span data-ttu-id="35a15-120">Arkistopostilaatikoiden ottaminen käyttöön</span><span class="sxs-lookup"><span data-stu-id="35a15-120">Enable archive mailboxes</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes)

- [<span data-ttu-id="35a15-121">Arkisto- ja poistokäytännön määrittäminen</span><span class="sxs-lookup"><span data-stu-id="35a15-121">Set up an archive and deletion policy</span></span>](https://docs.microsoft.com//office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes)
