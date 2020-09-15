---
title: Ulkopuolisten käyttäjien lisääminen jakeluun
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663510"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="47788-102">Lisää ulkoiset käyttäjät jako ryhmään</span><span class="sxs-lookup"><span data-stu-id="47788-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="47788-103">Ulkoisen yhteys henkilön lisääminen jakelu ryhmään (DG) on kaksivaiheinen prosessi:</span><span class="sxs-lookup"><span data-stu-id="47788-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="47788-104">Sähkö posti yhteys henkilön luominen ulkoiselle käyttäjälle:</span><span class="sxs-lookup"><span data-stu-id="47788-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="47788-105">Siirry hallinta keskuksessa **käyttäjät**-  >  [yhteys henkilöt](https://admin.microsoft.com/adminportal/home#/Contact) -sivulle.</span><span class="sxs-lookup"><span data-stu-id="47788-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="47788-106">Valitse **Lisää yhteys tieto**.</span><span class="sxs-lookup"><span data-stu-id="47788-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="47788-107">Kirjoita yhteys henkilön tiedot ja valitse **Lisää**.</span><span class="sxs-lookup"><span data-stu-id="47788-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="47788-108">Lisää Sähkö posti yhteys tieto PÄÄOSASTOOSI:</span><span class="sxs-lookup"><span data-stu-id="47788-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="47788-109">Siirry hallinta keskuksessa **ryhmät**  >  [ryhmät](https://admin.microsoft.com/adminportal/home#/groups) -sivulle.</span><span class="sxs-lookup"><span data-stu-id="47788-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="47788-110">Etsi pääosasto, johon haluat lisätä ulkoiset käyttäjät, ja valitse se avataksesi Muokkaa-valinta ikkunan.</span><span class="sxs-lookup"><span data-stu-id="47788-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="47788-111">Valitse **jäsenet** -väli lehdessä **Näytä kaikki ja Hallitse jäseniä**.</span><span class="sxs-lookup"><span data-stu-id="47788-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="47788-112">Valitse **Lisää jäseniä**.</span><span class="sxs-lookup"><span data-stu-id="47788-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="47788-113">Valitse edellisessä vaiheessa luomasi Sähkö posti yhteys tieto ja valitse sitten **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="47788-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="47788-114">Jos ulkoiset käyttäjät eivät voi lähettää sähkö posti viestejä pääosastolle tai eivät saa siitä Sähkö posti viestejä noudattamalla näitä ohjeita, voi olla, että pääosasto on merkitty sallimaan vain sisäisten käyttäjien lähettämät sähkö postit.</span><span class="sxs-lookup"><span data-stu-id="47788-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="47788-115">Voit tarkistaa tämän määrityksen ja korjata sen noudattamalla [tässä](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)annettuja ohjeita.</span><span class="sxs-lookup"><span data-stu-id="47788-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="47788-116">**Huomautus:** Näitä ohjeita ei sovelleta, jos ryhmän tyyppi on "Microsoft 365-ryhmä" eikä "Distribution Group".</span><span class="sxs-lookup"><span data-stu-id="47788-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="47788-117">Tässä tapa uksessa voit lisätä ulkoiset käyttäjät suoraan ryhmään Outlookista.</span><span class="sxs-lookup"><span data-stu-id="47788-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="47788-118">[Tässä artikkelissa](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)on lisä tietoja Microsoft 365-ryhmistä sekä ohjeita siitä, miten ulkoiset vieraat lisätään.</span><span class="sxs-lookup"><span data-stu-id="47788-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  