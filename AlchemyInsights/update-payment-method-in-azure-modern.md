---
title: Maksu tietojen päivittäminen Azuressa (moderni)
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 82c0a06e-86b0-4e8c-8644-59cbc02e7645
ms.custom:
- "9003546"
- "6857"
ms.openlocfilehash: bb032f772077318e54ac4fde42a72f432703d828
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807505"
---
# <a name="update-payment-details-in-azure"></a><span data-ttu-id="0ab87-102">Maksu tietojen päivittäminen Azure-tieto kannassa</span><span class="sxs-lookup"><span data-stu-id="0ab87-102">Update payment details in Azure</span></span>

<span data-ttu-id="0ab87-103">Jos luotto korttisi uusitaan ja numero pysyy samana, Päivitä nykyiset luotto kortti tiedot, kuten vanhenemis päivä.</span><span class="sxs-lookup"><span data-stu-id="0ab87-103">If your credit card gets renewed and the number stays the same, update the existing credit card details like the expiration date.</span></span> <span data-ttu-id="0ab87-104">Jos luotto korttisi numero muuttuu, koska kortti katoaa, varastetaan tai lakkaa, noudata [luotto kortin lisääminen maksu tavaksi](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support#addcard) -osiossa annettuja ohjeita.</span><span class="sxs-lookup"><span data-stu-id="0ab87-104">If your credit card number changes because the card is lost, stolen, or expired, follow the steps in the [Add a credit card as a payment method](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support#addcard) section.</span></span> <span data-ttu-id="0ab87-105">Sinun ei tarvitse päivittää CVV.</span><span class="sxs-lookup"><span data-stu-id="0ab87-105">You don't need to update the CVV.</span></span>

<span data-ttu-id="0ab87-106">Maksu tavat liittyvät [laskutus profiileihin](https://docs.microsoft.com/azure/billing/billing-how-to-change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support#change-payment-method-for-a-billing-profile).</span><span class="sxs-lookup"><span data-stu-id="0ab87-106">Your Payment methods are associated with [billing profiles](https://docs.microsoft.com/azure/billing/billing-how-to-change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support#change-payment-method-for-a-billing-profile).</span></span> <span data-ttu-id="0ab87-107">Vain Azuren rekisteröityneen käyttäjän ja laskutus tilin luonut käyttäjä voi päivittää maksu tapaa.</span><span class="sxs-lookup"><span data-stu-id="0ab87-107">Only the user who signed up for Azure and created the billing account can update the payment method.</span></span> <span data-ttu-id="0ab87-108">Päivitä maksu tapa noudattamalla näitä ohjeita.</span><span class="sxs-lookup"><span data-stu-id="0ab87-108">Follow these steps to update the payment method.</span></span>

1. <span data-ttu-id="0ab87-109">Kirjaudu sisään Azure- [portaaliin](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="0ab87-109">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="0ab87-110">Etsi **kustannusten hallinta + laskutus** .</span><span class="sxs-lookup"><span data-stu-id="0ab87-110">Search on **Cost Management + Billing** .</span></span>

3. <span data-ttu-id="0ab87-111">Valitse vasemmalla olevasta valikosta **laskutus profiilit** .</span><span class="sxs-lookup"><span data-stu-id="0ab87-111">In the menu on the left, select **Billing profiles** .</span></span>

4. <span data-ttu-id="0ab87-112">Valitse Laskutus profiili.</span><span class="sxs-lookup"><span data-stu-id="0ab87-112">Select a billing profile.</span></span>

5. <span data-ttu-id="0ab87-113">Valitse vasemmalla olevasta valikosta **Maksu tavat** .</span><span class="sxs-lookup"><span data-stu-id="0ab87-113">In the menu on the left, select **Payment methods** .</span></span>

6. <span data-ttu-id="0ab87-114">Etsi luotto **korttisi-osiossa luotto** kortti, jota haluat muokata.</span><span class="sxs-lookup"><span data-stu-id="0ab87-114">In the **Your credit cards** section, find the credit card you want to edit.</span></span>
7. <span data-ttu-id="0ab87-115">Valitse rivin lopussa kolme pistettä **(...)** .</span><span class="sxs-lookup"><span data-stu-id="0ab87-115">Select the ellipsis **(...)** at the end of the row.</span></span>

8. <span data-ttu-id="0ab87-116">Jos haluat muokata luotto korttisi tietoja, valitse pikavalikosta  **Muokkaa**  .</span><span class="sxs-lookup"><span data-stu-id="0ab87-116">To edit your credit card details, select  **Edit**  from the context menu.</span></span>
