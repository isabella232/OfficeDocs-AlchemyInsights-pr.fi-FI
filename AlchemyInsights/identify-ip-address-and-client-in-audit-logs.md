---
title: IP-osoite ja seurantalokeja asiakkaan tunnistaminen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1367
ms.assetid: ''
ms.openlocfilehash: 87e0d414fe02d5074a56cd5a77d50db1464b7faf
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752057"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="76af2-102">IP-osoite ja seurantalokeja asiakkaan tunnistaminen</span><span class="sxs-lookup"><span data-stu-id="76af2-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="76af2-103">IP-osoite, joka vastaa käyttäjän tai järjestelmänvalvojan tehtävä näkyy seurantalokit.</span><span class="sxs-lookup"><span data-stu-id="76af2-103">The IP address that corresponds to an activity by a user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="76af2-104">Asiakkaan tiedot kirjataan.</span><span class="sxs-lookup"><span data-stu-id="76af2-104">The client information is also logged.</span></span> <span data-ttu-id="76af2-105">Seuraavassa on ohjeita tällaisen tunnistetietoja</span><span class="sxs-lookup"><span data-stu-id="76af2-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="76af2-106">Kirjautua [Office 365-suojauksen & Compliance Centeriin](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="76af2-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="76af2-107">**Etsi ja tutkimus** ja valitse **Valvo lokista etsintää**.</span><span class="sxs-lookup"><span data-stu-id="76af2-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

   <span data-ttu-id="76af2-108">Jos olet kiinnostunut tietyn tehtävän, valitse **tehtävät** luettelosta.</span><span class="sxs-lookup"><span data-stu-id="76af2-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="76af2-109">Jos näin ei ole, palautetaan kaikki valitun käyttäjän (oletusasetus).</span><span class="sxs-lookup"><span data-stu-id="76af2-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="76af2-110">**Huomautus**: tietyt toimet eivät ole käytettävissä **toimintojen** valikon. kuitenkin ne valvottavat kohteet palautetaan Jos **Näytä tulokset kaikista** on valittuna (oletusasetus).</span><span class="sxs-lookup"><span data-stu-id="76af2-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="76af2-111">Määritä käyttäjänimi **käyttäjät** -kentässä ja valitse aktiviteetin päivämäärävälin **haku**.</span><span class="sxs-lookup"><span data-stu-id="76af2-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="76af2-112">Tulokset näet IP-osoitteen, että toiminnan tulokset-ruudussa.</span><span class="sxs-lookup"><span data-stu-id="76af2-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="76af2-113">Valitse asiakkuustietueen yksityiskohtaisia lisätietoja **tiedot** valikon avauspainike (esimerkiksi asiakas, käyttäjä, joka suorittaa toiminnon, jne.).</span><span class="sxs-lookup"><span data-stu-id="76af2-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="76af2-114">Lisätietoja [tartunnan saaneen tili käyttää tietokoneen IP-osoitteen löytäminen](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="76af2-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
