---
title: Ehdollisen käyttöoikeuden valvonta
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 374814f4eabd61433a15876ebf7f351819933c21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538739"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="281e8-102">Ehdollisen käyttöoikeuden Exchange seuranta</span><span class="sxs-lookup"><span data-stu-id="281e8-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="281e8-103">Kohdennetut ja ehdollisen käyttöoikeuden käyttäjät saavat sähköposti-ilmoitus, jos ne eivät täytä vaatimuksia organisaation. käyttö.</span><span class="sxs-lookup"><span data-stu-id="281e8-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="281e8-104">Ratkaisemiseksi, suosittelemme vähintään yksi seuraavista toimista:</span><span class="sxs-lookup"><span data-stu-id="281e8-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="281e8-105">Laite on rekisteröitynyt, siirry yritysportaalin yritys app ja varmista, että käyttäjä antaa neuvoja toteutuvan tulee yrityksen portaaliin.</span><span class="sxs-lookup"><span data-stu-id="281e8-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="281e8-106">Jos näin ei ole, käyttäjä pitäisi rekisteröidä laitteen.</span><span class="sxs-lookup"><span data-stu-id="281e8-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="281e8-107">Siirry portaalin Azure **Intune \> laitteen yhteensopivuuden**.</span><span class="sxs-lookup"><span data-stu-id="281e8-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="281e8-108">Valitse **näytön** **laitteen vaatimustenmukaisuus**.</span><span class="sxs-lookup"><span data-stu-id="281e8-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="281e8-109">Voit tarkastella laitteen yhteensopivuus raportin, varmista, että laitteen käyttäjän on merkitty niin paljon.</span><span class="sxs-lookup"><span data-stu-id="281e8-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="281e8-110">Siirry portaalin Azure **Intune \> laitteen yhteensopivuuden**.</span><span class="sxs-lookup"><span data-stu-id="281e8-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="281e8-111">Valitse **Hallitse** **käytäntöjä**.</span><span class="sxs-lookup"><span data-stu-id="281e8-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="281e8-112">Yhteensopivuuskäytäntöihin luettelossa Tarkista, että profiili on määritetty käyttäjän laitteeseen.</span><span class="sxs-lookup"><span data-stu-id="281e8-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="281e8-113">Jos ei ole profiilin on määritetty, Intune ei voi Vahvista laitteen yhteensopivuus tila.</span><span class="sxs-lookup"><span data-stu-id="281e8-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="281e8-114">Muokkaa käyttäjän ehdollisen käyttöoikeuden varauksen.</span><span class="sxs-lookup"><span data-stu-id="281e8-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="281e8-115">Siirry portaalin Azure **Intune \> ehdollisen käyttöoikeuden \> käytännöt**</span><span class="sxs-lookup"><span data-stu-id="281e8-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="281e8-116">Valitse käytäntö luettelosta</span><span class="sxs-lookup"><span data-stu-id="281e8-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="281e8-117">Valitse **käyttäjät ja ryhmät**</span><span class="sxs-lookup"><span data-stu-id="281e8-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="281e8-118">Joku on tiettyjä käytännön kohteeksi lisätä ne **luettelossa** .</span><span class="sxs-lookup"><span data-stu-id="281e8-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="281e8-119">Sen varmistamiseksi, että henkilö on pois käytännöstä, lisää ne **pois** luettelosta.</span><span class="sxs-lookup"><span data-stu-id="281e8-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="281e8-120">Lue lisää: [miten näyttö ehdollisen käyttöoikeuden laitteet](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="281e8-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

