---
title: Korttien ja maksutapojen hallinta
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003546"
- "6462"
ms.openlocfilehash: cfc4d84c8161c321a981eb5c4b0fb749c0c12047
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707987"
---
# <a name="manage-card-and-payment-method"></a><span data-ttu-id="2d828-102">Korttien ja maksutapojen hallinta</span><span class="sxs-lookup"><span data-stu-id="2d828-102">Manage Card and Payment Method</span></span>

<span data-ttu-id="2d828-103">Azure-portaalissa tilin järjestelmänvalvojana voit lisätä uuden debit-/credit-kortin, päivittää olemassa olevan debit-/credit card-kortin tai poistaa sellaisen debit/credit card -kortin, jota et käytä.</span><span class="sxs-lookup"><span data-stu-id="2d828-103">In the Azure portal, as an Account Administrator, you can add a new debit/credit card, update an existing debit/credit card, or delete a debit/credit card that you don't use.</span></span> <span data-ttu-id="2d828-104">[Microsoftin asiakassopimuksen maksutavat](https://docs.microsoft.com/azure/billing/billing-how-to-change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)liittyvät [laskutusprofiileihin.](https://docs.microsoft.com/azure/billing/billing-how-to-change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support#change-payment-method-for-a-billing-profile)</span><span class="sxs-lookup"><span data-stu-id="2d828-104">For [Microsoft Customer Agreement](https://docs.microsoft.com/azure/billing/billing-how-to-change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement), payment methods are associated with [billing profiles](https://docs.microsoft.com/azure/billing/billing-how-to-change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support#change-payment-method-for-a-billing-profile).</span></span> <span data-ttu-id="2d828-105">Vain Azureen rekisteröitynyt käyttäjä voi päivittää maksutapaa.</span><span class="sxs-lookup"><span data-stu-id="2d828-105">Only the user who signed up for Azure can update the payment method.</span></span>

<span data-ttu-id="2d828-106">**Uuden debit- tai credit card -kortin lisääminen Azure-tilaukseen**</span><span class="sxs-lookup"><span data-stu-id="2d828-106">**Add a new Debit or Credit card to an Azure Subscription**</span></span>

1. <span data-ttu-id="2d828-107">Kirjaudu Sisään [Azure-portaaliin](https://ms.portal.azure.com/) tilin [järjestelmänvalvojana.](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa) Valitse **Kustannusten hallinta + laskutus.**</span><span class="sxs-lookup"><span data-stu-id="2d828-107">Sign in to the [Azure portal](https://ms.portal.azure.com/) as the [Account Admin](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa). Select **Cost Management + Billing**.</span></span>
2. <span data-ttu-id="2d828-108">Valitse tilaus, jonne haluat lisätä debit- tai credit card -kortin.</span><span class="sxs-lookup"><span data-stu-id="2d828-108">Select a subscription you'd like to add the debit or credit card to.</span></span> <span data-ttu-id="2d828-109">Valitse **Maksutavat.**</span><span class="sxs-lookup"><span data-stu-id="2d828-109">Select **Payment methods**.</span></span>
3. <span data-ttu-id="2d828-110">Lisää kortti valitsemalla vasemmassa **+** yläkulmassa.</span><span class="sxs-lookup"><span data-stu-id="2d828-110">In the top-left corner, select **+** to add a card.</span></span> <span data-ttu-id="2d828-111">Oikealla näkyy debit/credit card -lomake.</span><span class="sxs-lookup"><span data-stu-id="2d828-111">A debit/credit card form will appear on the right.</span></span> <span data-ttu-id="2d828-112">Anna debit- tai credit card details (Pankki- tai luottokorttitiedot).</span><span class="sxs-lookup"><span data-stu-id="2d828-112">Enter debit or credit card details.</span></span>
4. <span data-ttu-id="2d828-113">Jos haluat tehdä tästä kortista aktiivisen  maksutavan, valitse lomakkeen yläosassa Tee tämä aktiivinen maksutapa -kohdan vieressä oleva valintaruutu.</span><span class="sxs-lookup"><span data-stu-id="2d828-113">To make this card your active payment method, check the box next to **Make this my active payment method** on top of the form.</span></span> <span data-ttu-id="2d828-114">Tästä kortista tulee aktiivinen maksuväline kaikissa tilauksia varten, jotka käyttävät samaa korttia kuin valittu tilaus.</span><span class="sxs-lookup"><span data-stu-id="2d828-114">This card will become the active payment instrument for all subscriptions that use the same card as the selected subscription.</span></span> <span data-ttu-id="2d828-115">Valitse **Seuraava**.</span><span class="sxs-lookup"><span data-stu-id="2d828-115">Select **Next**.</span></span>
5. <span data-ttu-id="2d828-116">Valitse **Aseta aktiivinen.**</span><span class="sxs-lookup"><span data-stu-id="2d828-116">Click **Set active**.</span></span> 
 
<span data-ttu-id="2d828-117">**Aiemmin luodun debit- tai credit card -kortin päivittäminen, muuttaminen tai poistaminen**</span><span class="sxs-lookup"><span data-stu-id="2d828-117">**Update/Change/Remove an existing Debit or Credit card**</span></span>

1.  <span data-ttu-id="2d828-118">Kirjaudu Sisään [Azure-portaaliin](https://portal.azure.com/) tilin [järjestelmänvalvojana.](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa) Hae kustannusten **hallintaa ja laskutusta.**</span><span class="sxs-lookup"><span data-stu-id="2d828-118">Sign in to the [Azure portal](https://portal.azure.com/) as the [Account Admin](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa). Search for **Cost Management + Billing**.</span></span>
2.  <span data-ttu-id="2d828-119">Valitse **Maksutavat.**</span><span class="sxs-lookup"><span data-stu-id="2d828-119">Select **Payment methods**.</span></span> <span data-ttu-id="2d828-120">Napsauta veloitus- tai luottokorttia, jota haluat muokata.</span><span class="sxs-lookup"><span data-stu-id="2d828-120">Click on the debit or credit card that you'd like to edit.</span></span> <span data-ttu-id="2d828-121">Oikealla näkyy debit/credit card -lomake.</span><span class="sxs-lookup"><span data-stu-id="2d828-121">A debit/credit card form will appear on the right.</span></span>
3.  <span data-ttu-id="2d828-122">Päivitä debit- tai credit card -tiedot.</span><span class="sxs-lookup"><span data-stu-id="2d828-122">Update the debit or credit card details.</span></span> <span data-ttu-id="2d828-123">Valitse **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="2d828-123">Select **Save**.</span></span>
4.  <span data-ttu-id="2d828-124">Jos **haluat** poistaa kortin, valitse sen kortin vieressä olevaa valintaruutua, jonka haluat poistaa.</span><span class="sxs-lookup"><span data-stu-id="2d828-124">To **remove**, check the box next to the card that you want to remove.</span></span>
5.  <span data-ttu-id="2d828-125">Valitse **Poista**.</span><span class="sxs-lookup"><span data-stu-id="2d828-125">Click **Delete**.</span></span>

<span data-ttu-id="2d828-126">**Huomautus:** Et voi poistaa pankkikorttiasi tai luottokorttiasi, jos se on liitetty muihin aktiivisten Microsoft-tilausten kanssa.</span><span class="sxs-lookup"><span data-stu-id="2d828-126">**Note**: You can't remove your debit/credit card if it is associated with other active Microsoft subscriptions.</span></span> <span data-ttu-id="2d828-127">Sinun on poistettava debit/credit card kaikista aktiivisista tilauksistasi Microsoftilla ja yritettävä uudelleen.</span><span class="sxs-lookup"><span data-stu-id="2d828-127">You will need to remove the debit/credit card from all active subscriptions that you have with Microsoft and try again.</span></span>

<span data-ttu-id="2d828-128">Lisätietoja on kohdassa [Maksutapojen päivittäminen, muuttaminen tai poistaminen](https://docs.microsoft.com/azure/billing/billing-how-to-change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="2d828-128">For more information, see [Update, change, or remove payment methods](https://docs.microsoft.com/azure/billing/billing-how-to-change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="2d828-129">**Maksuongelmien vianmääritys**</span><span class="sxs-lookup"><span data-stu-id="2d828-129">**Troubleshoot payment issues**</span></span>

<span data-ttu-id="2d828-130">Katso [maksuongelmien tai -virheskenaarioiden](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-troubleshoot-azure-payment-issues) vianmäärityksestä, ratkaiseeko ongelma ongelman.</span><span class="sxs-lookup"><span data-stu-id="2d828-130">Refer [Troubleshoot payment issues/error scenarios](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-troubleshoot-azure-payment-issues) to see if it resolves your issue.</span></span>

<span data-ttu-id="2d828-131">Jos kortissa on odottava maksu sen vuoksi, että rahoituslaitos hylkää korttisi, ota yhteyttä rahoituslaitostasi ongelman ratkaisemiseksi. </span><span class="sxs-lookup"><span data-stu-id="2d828-131">If there is a pending payment on the card as a result of your financial institution denying your card, please reach out to your **financial institution** to resolve the issue.</span></span> <span data-ttu-id="2d828-132">Käytä alla olevia osoitinta:</span><span class="sxs-lookup"><span data-stu-id="2d828-132">Use the below pointers:</span></span>

- <span data-ttu-id="2d828-133">Sinun täytyy ehkä tarkistaa pankki, jotta näet seuraavat:</span><span class="sxs-lookup"><span data-stu-id="2d828-133">You might have to check with the bank to see:</span></span> 
    - <span data-ttu-id="2d828-134">Jos kansainvälinen tapahtuma on otettu käyttöön kortissa</span><span class="sxs-lookup"><span data-stu-id="2d828-134">If the international transaction is enabled on the card</span></span>
    - <span data-ttu-id="2d828-135">Jos kortissa on saldon maksamiseen rajoitus</span><span class="sxs-lookup"><span data-stu-id="2d828-135">If card has credit limit to settle the balance</span></span>
    - <span data-ttu-id="2d828-136">Jos kortissa on käytössä toistuva maksu</span><span class="sxs-lookup"><span data-stu-id="2d828-136">If recurring payment is enabled on the card</span></span>

<span data-ttu-id="2d828-137">**Suositellut asiakirjat**</span><span class="sxs-lookup"><span data-stu-id="2d828-137">**Recommended Documents**</span></span>

- [<span data-ttu-id="2d828-138">Määritä laskutus</span><span class="sxs-lookup"><span data-stu-id="2d828-138">Set up invoicing</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/pay-by-invoice)
- [<span data-ttu-id="2d828-139">Vaihda maksutapaa – usein kysytyt kysymykset</span><span class="sxs-lookup"><span data-stu-id="2d828-139">Change payment method- FAQ</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions)
- [<span data-ttu-id="2d828-140">Laskutusprofiilin maksutavan muuttaminen</span><span class="sxs-lookup"><span data-stu-id="2d828-140">Change payment method for a billing profile</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support#change-payment-method-for-a-billing-profile)
- [<span data-ttu-id="2d828-141">Microsoftin asiakassopimuksen käytön tarkastaminen</span><span class="sxs-lookup"><span data-stu-id="2d828-141">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)
