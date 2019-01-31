---
title: Ehdollisen käyttöoikeuden valvonta
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: f4153f8a87a138d548c133142b0d48a319bd4b71
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656564"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="a3f06-102">Ehdollisen käyttöoikeuden valvonta</span><span class="sxs-lookup"><span data-stu-id="a3f06-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="a3f06-p101">Kohdennetut ja ehdollisen käyttöoikeuden käyttäjät saavat sähköposti-ilmoitus, jos ne eivät täytä vaatimuksia organisaation. käyttö. Ratkaisemiseksi, suosittelemme vähintään yksi seuraavista toimista:</span><span class="sxs-lookup"><span data-stu-id="a3f06-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="a3f06-p102">Laite on rekisteröitynyt, siirry yritysportaalin yritys app ja varmista, että käyttäjä antaa neuvoja toteutuvan tulee yrityksen portaaliin. Jos näin ei ole, käyttäjä pitäisi rekisteröidä laitteen.</span><span class="sxs-lookup"><span data-stu-id="a3f06-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="a3f06-p103">Siirry portaalin Azure **Intune \> laitteen yhteensopivuuden**. Valitse **näytön** **laitteen vaatimustenmukaisuus**. Voit tarkastella laitteen yhteensopivuus raportin, varmista, että laitteen käyttäjän on merkitty niin paljon.</span><span class="sxs-lookup"><span data-stu-id="a3f06-p103">In the Azure portal go to **Intune \> Device compliance**. Under **Monitor** click **Device compliance**. View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="a3f06-p104">Siirry portaalin Azure **Intune \> laitteen yhteensopivuuden**. Valitse **Hallitse** **käytäntöjä**. Yhteensopivuuskäytäntöihin luettelossa Tarkista, että profiili on määritetty käyttäjän laitteeseen. Jos ei ole profiilin on määritetty, Intune ei voi Vahvista laitteen yhteensopivuus tila.</span><span class="sxs-lookup"><span data-stu-id="a3f06-p104">In the Azure portal go to **Intune \> Device compliance**. Under **Manage**, click **Policies**. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="a3f06-114">Muokkaa käyttäjän ehdollisen käyttöoikeuden varauksen.</span><span class="sxs-lookup"><span data-stu-id="a3f06-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="a3f06-115">Siirry portaalin Azure **Intune \> ehdollisen käyttöoikeuden \> käytännöt**</span><span class="sxs-lookup"><span data-stu-id="a3f06-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="a3f06-116">Valitse käytäntö luettelosta</span><span class="sxs-lookup"><span data-stu-id="a3f06-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="a3f06-117">Valitse **käyttäjät ja ryhmät**</span><span class="sxs-lookup"><span data-stu-id="a3f06-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="a3f06-p105">Joku on tiettyjä käytännön kohteeksi lisätä ne **luettelossa** . Sen varmistamiseksi, että henkilö on pois käytännöstä, lisää ne **pois** luettelosta.</span><span class="sxs-lookup"><span data-stu-id="a3f06-p105">To target a certain policy at someone, add them to the **Include** list. To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="a3f06-120">Lue lisää: [miten näyttö ehdollisen käyttöoikeuden laitteet](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="a3f06-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

