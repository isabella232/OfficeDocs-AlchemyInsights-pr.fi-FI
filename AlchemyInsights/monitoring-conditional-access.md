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
ms.openlocfilehash: 756c5e98ed3e9cedd0152b5747ea6bf1ed31778e
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418466"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="edec3-102">Ehdollisen käyttöoikeuden valvonta</span><span class="sxs-lookup"><span data-stu-id="edec3-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="edec3-103">Kohdennetut ja ehdollisen käyttöoikeuden käyttäjät saavat sähköposti-ilmoitus, jos ne eivät täytä vaatimuksia organisaation. käyttö.</span><span class="sxs-lookup"><span data-stu-id="edec3-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="edec3-104">Ratkaisemiseksi, suosittelemme vähintään yksi seuraavista toimista:</span><span class="sxs-lookup"><span data-stu-id="edec3-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="edec3-105">Laite on rekisteröitynyt, siirry yritysportaalin yritys app ja varmista, että käyttäjä antaa neuvoja toteutuvan tulee yrityksen portaaliin.</span><span class="sxs-lookup"><span data-stu-id="edec3-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="edec3-106">Jos näin ei ole, käyttäjä pitäisi rekisteröidä laitteen.</span><span class="sxs-lookup"><span data-stu-id="edec3-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="edec3-107">Siirry portaalin Azure **Intune \> laitteen yhteensopivuuden**.</span><span class="sxs-lookup"><span data-stu-id="edec3-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="edec3-108">Valitse **näytön** **laitteen vaatimustenmukaisuus**.</span><span class="sxs-lookup"><span data-stu-id="edec3-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="edec3-109">Voit tarkastella laitteen yhteensopivuus raportin, varmista, että laitteen käyttäjän on merkitty niin paljon.</span><span class="sxs-lookup"><span data-stu-id="edec3-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="edec3-110">Siirry portaalin Azure **Intune \> laitteen yhteensopivuuden**.</span><span class="sxs-lookup"><span data-stu-id="edec3-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="edec3-111">Valitse **Hallitse** **käytäntöjä**.</span><span class="sxs-lookup"><span data-stu-id="edec3-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="edec3-112">Yhteensopivuuskäytäntöihin luettelossa Tarkista, että profiili on määritetty käyttäjän laitteeseen.</span><span class="sxs-lookup"><span data-stu-id="edec3-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="edec3-113">Jos ei ole profiilin on määritetty, Intune ei voi Vahvista laitteen yhteensopivuus tila.</span><span class="sxs-lookup"><span data-stu-id="edec3-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="edec3-114">Muokkaa käyttäjän ehdollisen käyttöoikeuden varauksen.</span><span class="sxs-lookup"><span data-stu-id="edec3-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="edec3-115">Siirry portaalin Azure **Intune \> ehdollisen käyttöoikeuden \> käytännöt**</span><span class="sxs-lookup"><span data-stu-id="edec3-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="edec3-116">Valitse käytäntö luettelosta</span><span class="sxs-lookup"><span data-stu-id="edec3-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="edec3-117">Valitse **käyttäjät ja ryhmät**</span><span class="sxs-lookup"><span data-stu-id="edec3-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="edec3-118">Joku on tiettyjä käytännön kohteeksi lisätä ne **luettelossa** .</span><span class="sxs-lookup"><span data-stu-id="edec3-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="edec3-119">Sen varmistamiseksi, että henkilö on pois käytännöstä, lisää ne **pois** luettelosta.</span><span class="sxs-lookup"><span data-stu-id="edec3-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="edec3-120">Lue lisää: [miten näyttö ehdollisen käyttöoikeuden laitteet](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="edec3-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

