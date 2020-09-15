---
title: IP-osoitteen ja asiakas ohjelman tunnistaminen valvonta lokeissa
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668307"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="27f1d-102">IP-osoitteen ja asiakas ohjelman tunnistaminen valvonta lokeissa</span><span class="sxs-lookup"><span data-stu-id="27f1d-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="27f1d-103">Microsoft 365-käyttäjän tai-järjestelmänvalvojan toimintaa vastaava IP-osoite näkyy valvonta lokeissa.</span><span class="sxs-lookup"><span data-stu-id="27f1d-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="27f1d-104">Myös asiakas tiedot kirjataan lokiin.</span><span class="sxs-lookup"><span data-stu-id="27f1d-104">The client information is also logged.</span></span> <span data-ttu-id="27f1d-105">Näiden tietojen tunnistamisen vaiheet</span><span class="sxs-lookup"><span data-stu-id="27f1d-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="27f1d-106">Kirjaudu sisään [Microsoft 365-tieto turva & Compliance Centeriin](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="27f1d-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="27f1d-107">Siirry **haun**  >  **valvonta lokien haku** sivulle.</span><span class="sxs-lookup"><span data-stu-id="27f1d-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="27f1d-108">Jos olet kiinnostunut tietystä aktiviteetista, valitse se **aktiviteetit** -luettelosta.</span><span class="sxs-lookup"><span data-stu-id="27f1d-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="27f1d-109">Jos näin ei ole, valitun käyttäjän kaikki toiminnot palautetaan (oletus asetus).</span><span class="sxs-lookup"><span data-stu-id="27f1d-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="27f1d-110">**Huomautus**: tietyt toiminnot eivät ehkä ole käytettävissä **aktiviteetit** -valikossa. Nämä valvonta kohteet palautetaan, jos **kaikkien aktiviteettien Näytä tulokset** -vaihto ehto on valittuna (oletus asetus).</span><span class="sxs-lookup"><span data-stu-id="27f1d-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="27f1d-111">Määritä käyttäjä nimi **käyttäjät** -kentässä, valitse aktiviteetille sopiva päivämäärä alue ja valitse sitten **Hae**.</span><span class="sxs-lookup"><span data-stu-id="27f1d-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="27f1d-112">Tuloksissa näkyy kyseisen toiminnon IP-osoite tulokset-ruudussa.</span><span class="sxs-lookup"><span data-stu-id="27f1d-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="27f1d-113">Valitse valvonta tietue, jos haluat nähdä yksityiskohtaisia tietoja tietojen pikavalikosta (esimerkiksi asiakas, käyttäjä, **joka on suorittanut** toiminnon jne.).</span><span class="sxs-lookup"><span data-stu-id="27f1d-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="27f1d-114">Lisä tietoja on kohdassa [sen tieto koneen IP-osoitteen etsiminen, jota käytetään vaarantuneen tilin käyttämiseen](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="27f1d-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
