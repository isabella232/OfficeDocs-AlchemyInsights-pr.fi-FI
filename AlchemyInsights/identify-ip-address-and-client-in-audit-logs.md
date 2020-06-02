---
title: IP-osoitteen ja asiakkaan tunnistaminen valvontalokeissa
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 80b652eb65612093252dee226a19ec74bc035faa
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508913"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="fd75f-102">IP-osoitteen ja asiakkaan tunnistaminen valvontalokeissa</span><span class="sxs-lookup"><span data-stu-id="fd75f-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="fd75f-103">Microsoft 365 -käyttäjän tai -järjestelmänvalvojan toimintaa vastaava IP-osoite näkyy valvontalokeissa.</span><span class="sxs-lookup"><span data-stu-id="fd75f-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="fd75f-104">Myös asiakastiedot kirjataan lokiin.</span><span class="sxs-lookup"><span data-stu-id="fd75f-104">The client information is also logged.</span></span> <span data-ttu-id="fd75f-105">Tässä ovat vaiheet tällaisten tietojen tunnistamiseksi</span><span class="sxs-lookup"><span data-stu-id="fd75f-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="fd75f-106">Kirjaudu Microsoft [365 Security & Compliance Centeriin.](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="fd75f-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="fd75f-107">Siirry **Haun**  >  **valvontalokin hakusivulle.**</span><span class="sxs-lookup"><span data-stu-id="fd75f-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="fd75f-108">Jos olet kiinnostunut tietystä aktiviteetista, valitse se **Aktiviteetit-luettelosta.**</span><span class="sxs-lookup"><span data-stu-id="fd75f-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="fd75f-109">Jos näin ei ole, kaikki aktiviteetit palautetaan valitulle käyttäjälle (oletusasetus).</span><span class="sxs-lookup"><span data-stu-id="fd75f-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="fd75f-110">**Huomautus:** Tietyt toiminnot eivät ehkä ole käytettävissä **Aktiviteetit-valikossa.** Nämä valvontakohteet palautetaan kuitenkin, jos **Näytä kaikkien aktiviteettien tulokset** on valittuna (oletusasetus).</span><span class="sxs-lookup"><span data-stu-id="fd75f-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="fd75f-111">Määritä käyttäjänimi Käyttäjät-kentässä, valitse aktiviteetille sopiva päivämääräalue ja valitse sitten **Etsi**. **Users**</span><span class="sxs-lookup"><span data-stu-id="fd75f-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="fd75f-112">Tuloksissa näet kyseisen aktiviteetin IP-osoitteen tulosruudussa.</span><span class="sxs-lookup"><span data-stu-id="fd75f-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="fd75f-113">Valitse valvontatietue, jos haluat nähdä yksityiskohtaiset tiedot **Tiedot-pikaikkunassa** (esimerkiksi Asiakas, Käyttäjä, joka suoritti toiminnon jne.).</span><span class="sxs-lookup"><span data-stu-id="fd75f-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="fd75f-114">Lisätietoja on [ohjeaiheessa Vaarantuneen tilin käyttämiseen käytettävän tietokoneen IP-osoitteen etsiminen](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="fd75f-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
