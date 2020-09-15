---
title: 618-kalenterin jakamis käytännöt
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684227"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="7e44b-102">Käytäntöä koskeva virhe kalenteria jaettaessa</span><span class="sxs-lookup"><span data-stu-id="7e44b-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="7e44b-103">Tee tilan teen mukaan jokin seuraavista:</span><span class="sxs-lookup"><span data-stu-id="7e44b-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="7e44b-104">Muodosta yhteys Exchange Onlineen PowerShell-etätoiminnolla.</span><span class="sxs-lookup"><span data-stu-id="7e44b-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="7e44b-105">Lisä tietoja on Ohje aiheessa [yhteyden muodostaminen Exchange Onlineen PowerShellin etätoiminnolla](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="7e44b-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="7e44b-106">Avaa Exchange-hallinta liittymä paikallisessa palvelimessa.</span><span class="sxs-lookup"><span data-stu-id="7e44b-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="7e44b-107">Määrittää käyttäjälle määritetyn jakamis käytäntöjen.</span><span class="sxs-lookup"><span data-stu-id="7e44b-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="7e44b-108">Jos haluat tehdä tämän, suorita seuraava komento ja huomioi sen palauttama menettely:</span><span class="sxs-lookup"><span data-stu-id="7e44b-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="7e44b-109">Päivitä käyttäjän jakamis käytäntöä.</span><span class="sxs-lookup"><span data-stu-id="7e44b-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="7e44b-110">Voit tehdä tämän seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="7e44b-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="7e44b-111">Avaa Exchange-hallinta keskus.</span><span class="sxs-lookup"><span data-stu-id="7e44b-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="7e44b-112">Valitse **organisaatio**ja kaksoisnapsauta sitten **yksittäistä jakoa**varten määritettyä käytäntöä.</span><span class="sxs-lookup"><span data-stu-id="7e44b-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="7e44b-113">Tämä on vaiheessa 2 palautettu käytännöt.</span><span class="sxs-lookup"><span data-stu-id="7e44b-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="7e44b-114">Valitse jakamis sääntö-sivulla sen kalenterin jakamis taso, jonka haluat sallia, kohdassa Määritä, **mitä tietoja haluat jakaa**. Valitse **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="7e44b-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="7e44b-115">Lisä tietoja on kohdassa ["käytännöt eivät salli oikeuksien myöntämistä tällä tasolla yhdelle tai useammalle vastaanottajalle"-virhe, kun käyttäjä yrittää jakaa kalenteria](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="7e44b-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
