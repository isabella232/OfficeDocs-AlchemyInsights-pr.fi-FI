---
title: Ulkoisten käyttäjien lisääminen jakeluryhmään
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910929"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="c720c-102">Ulkoisten käyttäjien lisääminen jakeluryhmään</span><span class="sxs-lookup"><span data-stu-id="c720c-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="c720c-103">Ulkoisen yhteyshenkilön lisääminen jakeluryhmään on kaksivaiheinen prosessi:</span><span class="sxs-lookup"><span data-stu-id="c720c-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="c720c-104">Luo sähköpostiyhteystieto ulkoiselle käyttäjälle:</span><span class="sxs-lookup"><span data-stu-id="c720c-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="c720c-105">Siirry hallintakeskuksessa **Käyttäjien** > [yhteystiedot -sivulle.](https://admin.microsoft.com/adminportal/home#/Contact)</span><span class="sxs-lookup"><span data-stu-id="c720c-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="c720c-106">Valitse **Lisää yhteystieto**.</span><span class="sxs-lookup"><span data-stu-id="c720c-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="c720c-107">Kirjoita yhteyshenkilön tiedot ja valitse **Lisää**.</span><span class="sxs-lookup"><span data-stu-id="c720c-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="c720c-108">Lisää sähköpostiyhteystieto pääosastoosi:</span><span class="sxs-lookup"><span data-stu-id="c720c-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="c720c-109">Siirry hallintakeskuksessa **Ryhmät ryhmät** > [-sivulle.](https://admin.microsoft.com/adminportal/home#/groups)</span><span class="sxs-lookup"><span data-stu-id="c720c-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="c720c-110">Etsi pääosasto, jolle haluat lisätä ulkoisen käyttäjän, ja avaa muokkausikkuna valitsemalla se.</span><span class="sxs-lookup"><span data-stu-id="c720c-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="c720c-111">Valitse **Jäsenet-välilehdessä** **Näytä kaikki ja hallitse jäseniä**.</span><span class="sxs-lookup"><span data-stu-id="c720c-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="c720c-112">Valitse **Lisää jäseniä**.</span><span class="sxs-lookup"><span data-stu-id="c720c-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="c720c-113">Valitse edellisessä vaiheessa luomasi sähköpostiyhteystieto ja valitse sitten **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="c720c-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="c720c-114">Jos ulkoiset käyttäjät eivät voi näiden vaiheiden jälkeen lähettää sähköposteja pääosastolle tai vastaanottaa siitä sähköposteja, voi olla, että pääosasto on merkitty sallimaan vain sisäisten käyttäjien sähköpostit.</span><span class="sxs-lookup"><span data-stu-id="c720c-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="c720c-115">Voit tarkistaa tämän kokoonpanon ja korjata sen noudattamalla ohjeita [täällä](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="c720c-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="c720c-116">**Huomautus:** Nämä ohjeet eivät päde, jos ryhmän tyyppi on Jakeluryhmä-asetuksen sijasta Microsoft 365 -ryhmä.</span><span class="sxs-lookup"><span data-stu-id="c720c-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="c720c-117">Jos näin on, voit lisätä ulkoisen käyttäjän suoraan ryhmään Outlookista.</span><span class="sxs-lookup"><span data-stu-id="c720c-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="c720c-118">Tässä [artikkelissa](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)on yksityiskohtaisia tietoja Microsoft 365 Groupsin vieraista sekä ohjeet ulkoisten vieraiden lisäämiseen.</span><span class="sxs-lookup"><span data-stu-id="c720c-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  