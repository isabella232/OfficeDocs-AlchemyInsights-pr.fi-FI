---
title: Arkisto posti laatikon ottaminen käyttöön
ms.author: markjjo
author: markjjo
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "307"
- "3100008"
ms.assetid: e1a5fab7-d3a5-4d4c-8ee2-0edf4ec9b76b
ms.openlocfilehash: 3e20eaf8dec85454ce5a67e1b21292b2a33ebb1d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47811702"
---
# <a name="enable-an-archive-mailbox"></a><span data-ttu-id="fbd0a-102">Arkisto posti laatikon ottaminen käyttöön</span><span class="sxs-lookup"><span data-stu-id="fbd0a-102">Enable an archive mailbox</span></span>

<span data-ttu-id="fbd0a-103">Jos haluat, että suoritat automaattiset tarkistukset varmistaaksesi, että Arkisto posti laatikko voidaan määrittää, valitse Edellinen-painike <--tämän sivun yläosassa ja kirjoita sitten tilin Sähkö posti osoite.</span><span class="sxs-lookup"><span data-stu-id="fbd0a-103">If you want us to run automated checks to ensure an archive mailbox can be configured, select the back button <-- at the top of this page, and then enter the email address of the account.</span></span>

<span data-ttu-id="fbd0a-104">Posti laatikoiden arkistoiminen Microsoft 365 (kutsutaan myös *online-arkistoihin* tai *in-Place-arkistoihin*) Lisää sähkö postin tallennus tilaa käyttäjille.</span><span class="sxs-lookup"><span data-stu-id="fbd0a-104">Archive mailboxes in Microsoft 365 (also called *Online Archives* or *In-Place Archives*) provide users with additional email storage.</span></span> <span data-ttu-id="fbd0a-105">Käyttäjät voivat siirtää tai kopioida kohteita Arkisto posti laatikkoon, ja järjestelmänvalvojat voivat luoda arkistointi käytäntöjä, jotka siirtävät kohteet automaattisesti Arkisto posti laatikoihin.</span><span class="sxs-lookup"><span data-stu-id="fbd0a-105">Users can move or copy items to their archive mailbox, and admins can create an archive policy that automatically moves items to archive mailboxes.</span></span>
  
<span data-ttu-id="fbd0a-106">Voit luoda Arkisto posti laatikon seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="fbd0a-106">Here's how to create an archive mailbox:</span></span>
  
1. <span data-ttu-id="fbd0a-107">Siirry osoitteeseen [https://protection.office.com](https://protection.office.com).</span><span class="sxs-lookup"><span data-stu-id="fbd0a-107">Go to [https://protection.office.com](https://protection.office.com).</span></span>

2. <span data-ttu-id="fbd0a-108">Kirjaudu sisään Microsoft 365-tiliisi käyttämällä järjestelmänvalvojan tiliä.</span><span class="sxs-lookup"><span data-stu-id="fbd0a-108">Sign in to Microsoft 365 using your admin account.</span></span>

3. <span data-ttu-id="fbd0a-109">Valitse tieto turva &amp; -yhteensopivuus keskuksen vasemmanpuoleisesta ruudusta **tietojen hallinta** - \> **Arkisto**.</span><span class="sxs-lookup"><span data-stu-id="fbd0a-109">In the left pane of the Security &amp; Compliance Center, select **Information governance** \> **Archive**.</span></span>

4. <span data-ttu-id="fbd0a-110">Valitse käyttäjä, jonka Arkisto posti laatikon haluat ottaa käyttöön.</span><span class="sxs-lookup"><span data-stu-id="fbd0a-110">Select the user whose archive mailbox you want to enable.</span></span>

5. <span data-ttu-id="fbd0a-111">Valitse oikealla olevassa tieto ruudussa **Ota käyttöön** ja ota Arkisto posti laatikko käyttöön napsauttamalla varoitus viestissä **Kyllä** .</span><span class="sxs-lookup"><span data-stu-id="fbd0a-111">In the details pane on the right, click **Enable** and then click **Yes** in the warning message to enable the archive mailbox.</span></span>

<span data-ttu-id="fbd0a-112">Voit myös ottaa Arkisto posti laatikot joukkona käyttöön valitsemalla useita käyttäjiä (käyttämällä **vaihto** -tai **CTRL** -näppäimiä) ja valitsemalla sitten tieto ruudussa **Ota käyttöön** .</span><span class="sxs-lookup"><span data-stu-id="fbd0a-112">You can also bulk-enable archive mailboxes by selecting multiple users (using the **Shift** or **Ctrl** keys) and then clicking **Enable** in the details pane.</span></span>
  
### <a name="shared-mailboxes"></a><span data-ttu-id="fbd0a-113">Jaetut postilaatikot</span><span class="sxs-lookup"><span data-stu-id="fbd0a-113">Shared mailboxes</span></span>

<span data-ttu-id="fbd0a-114">Jos haluat ottaa käyttöön arkiston jaetulle posti laatikolle, Exchange Online-tila uksen 2 käyttö oikeus tai Exchange Online-käyttö oikeus sopimus 1-lisenssi edellyttää Exchange Online-arkistointi käyttö oikeutta.</span><span class="sxs-lookup"><span data-stu-id="fbd0a-114">To enable the archive for a shared mailbox, an Exchange Online Plan 2 license or an Exchange Online Plan 1 license with an Exchange Online Archiving license is required.</span></span>  

<span data-ttu-id="fbd0a-115">Jos haluat ottaa käyttöön arkiston jaetulle posti laatikolle:</span><span class="sxs-lookup"><span data-stu-id="fbd0a-115">To enable the archive for a shared mailbox:</span></span>

1. <span data-ttu-id="fbd0a-116">Siirry Exchange- [hallinta keskukseen](https://outlook.office365.com/ecp) ja Kirjaudu sisään käyttämällä järjestelmänvalvojan tiliä.</span><span class="sxs-lookup"><span data-stu-id="fbd0a-116">Go to the [Exchange admin center](https://outlook.office365.com/ecp) and sign in using your admin account.</span></span>

2. <span data-ttu-id="fbd0a-117">Siirry **Recipients**  >  **jaettavat**vastaanottajat-kohtaan.</span><span class="sxs-lookup"><span data-stu-id="fbd0a-117">Go to **Recipients** > **Shared**.</span></span>

3. <span data-ttu-id="fbd0a-118">Valitse jaettava posti laatikko.</span><span class="sxs-lookup"><span data-stu-id="fbd0a-118">Select the shared mailbox.</span></span>

4. <span data-ttu-id="fbd0a-119">Valitse oikealla olevan tiedot **-ruudun kohta Arkisto**-kohdassa **Ota käyttöön**ja valitse sitten **Kyllä** , jos haluat ottaa Arkisto posti laatikon käyttöön.</span><span class="sxs-lookup"><span data-stu-id="fbd0a-119">In the details pane on the right, under **In-Place Archive**, click **Enable**, and then click **Yes** to enable the archive mailbox.</span></span>

<span data-ttu-id="fbd0a-120">Lisätietoja on seuraavissa artikkeleissa:</span><span class="sxs-lookup"><span data-stu-id="fbd0a-120">For more information, see:</span></span>
  
- [<span data-ttu-id="fbd0a-121">Arkisto posti laatikoiden ottaminen käyttöön</span><span class="sxs-lookup"><span data-stu-id="fbd0a-121">Enable archive mailboxes</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes)

- [<span data-ttu-id="fbd0a-122">Arkistointi-ja poisto käytäntöjen määrittäminen</span><span class="sxs-lookup"><span data-stu-id="fbd0a-122">Set up an archive and deletion policy</span></span>](https://docs.microsoft.com//office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes)
