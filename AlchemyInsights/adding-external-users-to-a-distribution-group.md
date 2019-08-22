---
title: Ulkoisten käyttäjien lisääminen jakeluryhmään
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 8/22/2017
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: ce0c589e1661fb4607452fe2e8f897758b2718e8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36494524"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="5a9cd-102">Ulkoisten käyttäjien lisääminen jakeluryhmän?</span><span class="sxs-lookup"><span data-stu-id="5a9cd-102">Add external users to a Distribution Group?</span></span>

<span data-ttu-id="5a9cd-103">Lisäämällä ulkoinen kontakti, jakelu ryhmä (Po) on 2 vaiheessa:</span><span class="sxs-lookup"><span data-stu-id="5a9cd-103">Adding an external contact to a Distribution Group (DG) is a 2-step process:</span></span>
  
1. <span data-ttu-id="5a9cd-104">Luo ulkoisen käyttäjän yhteyshenkilön sähköposti:</span><span class="sxs-lookup"><span data-stu-id="5a9cd-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="5a9cd-105">Siirry hallintakeskukseen, **käyttäjien** > [yhteyshenkilöt](https://admin.microsoft.com/adminportal/home#/Contact) -sivu.</span><span class="sxs-lookup"><span data-stu-id="5a9cd-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="5a9cd-106">Valitse **Lisää henkilö**.</span><span class="sxs-lookup"><span data-stu-id="5a9cd-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="5a9cd-107">Kirjoita yhteyshenkilösi tiedot ja valitse **Lisää**.</span><span class="sxs-lookup"><span data-stu-id="5a9cd-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="5a9cd-108">Lisää oman Po yhteyshenkilön sähköposti:</span><span class="sxs-lookup"><span data-stu-id="5a9cd-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="5a9cd-109">Siirry hallintakeskukseen, **ryhmiä** > [ryhmät](https://admin.microsoft.com/adminportal/home#/groups) -sivulla.</span><span class="sxs-lookup"><span data-stu-id="5a9cd-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="5a9cd-110">Etsi Po, johon haluat lisätä ulkoisen käyttäjän, ja valitse Avaa valintaikkunan Muokkaa.</span><span class="sxs-lookup"><span data-stu-id="5a9cd-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="5a9cd-111">Valitse **jäsenet** -välilehdessä **Hallitse jäseniä ja tarkastella kaikkia**.</span><span class="sxs-lookup"><span data-stu-id="5a9cd-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="5a9cd-112">Valitse **Lisää jäseniä**.</span><span class="sxs-lookup"><span data-stu-id="5a9cd-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="5a9cd-113">Valitse Mail edellisessä vaiheessa luomaasi yhteystietoa ja valitse sitten **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="5a9cd-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="5a9cd-114">Jos jälkeen seuraavat toimet ulkoisten käyttäjien Po ei voi lähettää sähköpostia tai et voi vastaanottaa sähköpostit sitä, voi olla Po on merkitty Salli vain sisäisten käyttäjien sähköpostit.</span><span class="sxs-lookup"><span data-stu-id="5a9cd-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="5a9cd-115">Voit tarkistaa tämän kokoonpanon ja se helppoa korjata [tätä](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).</span><span class="sxs-lookup"><span data-stu-id="5a9cd-115">You can check this configuration and fix it following the directions [here](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).</span></span>
  
 <span data-ttu-id="5a9cd-116">**Huomautus:** Älä käytä näitä ohjeita, jos ryhmän tyyppi on ”Office 365-ryhmä” sijasta ”jakeluryhmä”.</span><span class="sxs-lookup"><span data-stu-id="5a9cd-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="5a9cd-117">Jos näin on, voit lisätä ulkoinen käyttäjä ryhmään suoraan Outlookista.</span><span class="sxs-lookup"><span data-stu-id="5a9cd-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="5a9cd-118">Office 365-ryhmien vieraita koskevat yksityiskohtaiset tiedot sekä lisäämällä ulkoisen vieraat ohjeet löytyy [tämän](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)artikkelin.</span><span class="sxs-lookup"><span data-stu-id="5a9cd-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  