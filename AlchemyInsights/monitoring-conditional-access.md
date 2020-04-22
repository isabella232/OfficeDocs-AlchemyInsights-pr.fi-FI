---
title: Ehdollisen käytön valvonta
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713715"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="46fdc-102">Ehdollisen käytön valvonta Exchangessa</span><span class="sxs-lookup"><span data-stu-id="46fdc-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="46fdc-103">Ehdolliseen käyttöön kohdistetut käyttäjät saavat sähköposti-ilmoituksen, jos he eivät täytä organisaatiosi käyttövaatimuksia.</span><span class="sxs-lookup"><span data-stu-id="46fdc-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="46fdc-104">Ratkaisua suositellaan vähintään yhtä seuraavista ratkaisuista:</span><span class="sxs-lookup"><span data-stu-id="46fdc-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="46fdc-105">Jos laitteen oletetaan olevan rekisteröitynyt, kehota käyttäjää menemään Yritysportaali-sovellukseen ja varmistamaan, että se näkyy yritysportaalissa.</span><span class="sxs-lookup"><span data-stu-id="46fdc-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="46fdc-106">Jos näin ei ole, käyttäjän on rekisteröitava laite.</span><span class="sxs-lookup"><span data-stu-id="46fdc-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="46fdc-107">Siirry Azure-portaalissa **Kohtaan \> Intune Device compliance**.</span><span class="sxs-lookup"><span data-stu-id="46fdc-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="46fdc-108">Valitse **Näyttö-kohdassa** **Laitteen yhteensopivuus**.</span><span class="sxs-lookup"><span data-stu-id="46fdc-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="46fdc-109">Tarkista laitteen yhteensopivuusraportista, että käyttäjän laite on merkitty yhteensopivaksi.</span><span class="sxs-lookup"><span data-stu-id="46fdc-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="46fdc-110">Siirry Azure-portaalissa **Kohtaan \> Intune Device compliance**.</span><span class="sxs-lookup"><span data-stu-id="46fdc-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="46fdc-111">Valitse **Hallinta**-kohdassa **Käytännöt**.</span><span class="sxs-lookup"><span data-stu-id="46fdc-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="46fdc-112">Varmista yhteensopivuuskäytäntöjen luettelosta, että käyttäjän laitteelle on määritetty profiili.</span><span class="sxs-lookup"><span data-stu-id="46fdc-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="46fdc-113">Jos profiilia ei ole määritetty, Intune ei voi vahvistaa laitteen vaatimustenmukaisuuden tilaa.</span><span class="sxs-lookup"><span data-stu-id="46fdc-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="46fdc-114">Muokkaa käyttäjän ehdollisen käytön määritystä.</span><span class="sxs-lookup"><span data-stu-id="46fdc-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="46fdc-115">Siirry Azure-portaalissa **Intune-ehdollisen \> käytön \> käytäntöihin**</span><span class="sxs-lookup"><span data-stu-id="46fdc-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="46fdc-116">Käytännön valitseminen luettelosta</span><span class="sxs-lookup"><span data-stu-id="46fdc-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="46fdc-117">Valitse **Käyttäjät ja ryhmät.**</span><span class="sxs-lookup"><span data-stu-id="46fdc-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="46fdc-118">Jos haluat kohdistaa tietyn käytännön johonkin, lisää hänet **Sisällytä-luetteloon.**</span><span class="sxs-lookup"><span data-stu-id="46fdc-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="46fdc-119">Voit varmistaa, että henkilö jätetään pois käytännöstä, lisäämällä hänet **Pois-luetteloon.**</span><span class="sxs-lookup"><span data-stu-id="46fdc-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="46fdc-120">Lue lisää: [Ehdollisen käytön laitteiden valvonta](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="46fdc-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

