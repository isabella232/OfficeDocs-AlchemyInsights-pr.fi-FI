---
title: Ehdollisen käytön valvominen
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702900"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="e8447-102">Ehdollisen Exchange-yhteyden valvonta</span><span class="sxs-lookup"><span data-stu-id="e8447-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="e8447-103">Ehdolliseen käyttöön kohdistetut käyttäjät saavat ilmoitus Sähkö posti viestin, jos he eivät täytä organisaatiosi käyttö oikeus vaatimuksia.</span><span class="sxs-lookup"><span data-stu-id="e8447-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="e8447-104">Ratkaisu on suositeltava vähintään yksi seuraavista ratkaisuista:</span><span class="sxs-lookup"><span data-stu-id="e8447-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="e8447-105">Jos laitteen oletetaan olevan rekisteröity, kehota käyttäjää siirtymään yritys portaali-sovellukseen ja vahvistamaan, että se näkyy yritys portaalissa.</span><span class="sxs-lookup"><span data-stu-id="e8447-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="e8447-106">Jos näin ei tapahdu, käyttäjän on rekisteröitävä laite.</span><span class="sxs-lookup"><span data-stu-id="e8447-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="e8447-107">Valitse Azure-portaalissa **Intune- \> laitteen yhteensopivuus**.</span><span class="sxs-lookup"><span data-stu-id="e8447-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="e8447-108">Valitse **näyttö** -kohdassa **laitteen yhteensopivuus**.</span><span class="sxs-lookup"><span data-stu-id="e8447-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="e8447-109">Tarkastele laitteesi yhteensopivuus raporttia varmistaaksesi, että käyttäjän laite on merkitty yhteensopivaksi.</span><span class="sxs-lookup"><span data-stu-id="e8447-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="e8447-110">Valitse Azure-portaalissa **Intune- \> laitteen yhteensopivuus**.</span><span class="sxs-lookup"><span data-stu-id="e8447-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="e8447-111">Valitse **hallinta**-kohdassa **käytännöt**.</span><span class="sxs-lookup"><span data-stu-id="e8447-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="e8447-112">Varmista yhteensopivuus käytäntöjen luettelosta, että profiili on määritetty käyttäjän laitteelle.</span><span class="sxs-lookup"><span data-stu-id="e8447-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="e8447-113">Jos profiilia ei ole määritetty, Intune ei pysty vahvistamaan laitteen yhteensopivuus tilaa.</span><span class="sxs-lookup"><span data-stu-id="e8447-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="e8447-114">Muokkaa käyttäjän ehdollisen käytön määritystä.</span><span class="sxs-lookup"><span data-stu-id="e8447-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="e8447-115">Azure-portaalissa Siirry **Intune-sivuston \> ehdollisen käytön \> käytäntöihin**</span><span class="sxs-lookup"><span data-stu-id="e8447-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="e8447-116">Valitse käytännöstä luettelosta</span><span class="sxs-lookup"><span data-stu-id="e8447-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="e8447-117">Valitse **käyttäjät ja ryhmät**</span><span class="sxs-lookup"><span data-stu-id="e8447-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="e8447-118">Jos haluat kohdentaa tiettyyn käytäntöön jollekulle, lisää ne **Sisällytä** -luetteloon.</span><span class="sxs-lookup"><span data-stu-id="e8447-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="e8447-119">Jos haluat varmistaa, että henkilö jätetään pois käytännöstä, Lisää hänet **Jätä pois** -luetteloon.</span><span class="sxs-lookup"><span data-stu-id="e8447-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="e8447-120">Lue lisää: [ehdollisen pääsyn valvonta laitteiden valvominen](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="e8447-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

