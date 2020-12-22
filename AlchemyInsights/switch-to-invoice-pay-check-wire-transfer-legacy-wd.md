---
title: Siirry lasku maksuun (sekki/pankki siirto) – aiempi WD
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
- "9004168"
- "7343"
ms.openlocfilehash: 1be90771f994e832960383b1cb5e0bee8f5b08f8
ms.sourcegitcommit: b561c339926fad609950ac92744c3cd91e0a68fa
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/21/2020
ms.locfileid: "49726128"
---
# <a name="switch-to-invoice-pay-chequewire-transfer---legacy-wd"></a><span data-ttu-id="f1f5c-102">Siirry lasku maksuun (sekki/pankki siirto) – aiempi WD</span><span class="sxs-lookup"><span data-stu-id="f1f5c-102">Switch to invoice pay (cheque/wire transfer) - Legacy WD</span></span>

<span data-ttu-id="f1f5c-103">Jos vaihdat maksa maan laskulla, maksat laskun 30 päivän kuluessa laskun päivä määrästä.</span><span class="sxs-lookup"><span data-stu-id="f1f5c-103">If you switch to pay by invoice, that means you will pay your bill within 30 days of the invoice date.</span></span> <span data-ttu-id="f1f5c-104">Jos haluat, että olet oikeutettu maksa maan Azure-tilauksestasi laskulla, Lähetä pyyntö Azure-tukeen.</span><span class="sxs-lookup"><span data-stu-id="f1f5c-104">To become eligible to pay for your Azure subscription by invoice, submit a request to Azure support.</span></span> <span data-ttu-id="f1f5c-105">Kun pyyntösi on hyväksytty, voit vaihtaa tila uksen lasku maksuun [Azure-portaalissa](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="f1f5c-105">Once your request is approved, you can switch a subscription to invoice pay in the [Azure portal](https://portal.azure.com/).</span></span>

<span data-ttu-id="f1f5c-106">**Ennen kuin jatkat, tarkista seuraavat ehdot/rajoitukset, jotka koskevat laskun maksu tapaa:**</span><span class="sxs-lookup"><span data-stu-id="f1f5c-106">**Before you proceed further, review the following requirements/limitations on requesting invoice payment option:**</span></span>

- <span data-ttu-id="f1f5c-107">Kirjaudu sisään [Azure Portaliin](https://portal.azure.com/) ja siirry maksu tapoihin.</span><span class="sxs-lookup"><span data-stu-id="f1f5c-107">Log in to [Azure portal](https://portal.azure.com/) and navigate to payment methods.</span></span> <span data-ttu-id="f1f5c-108">Tarkista, onko laskutus maksussa jo valmiiksi hyväksytty.</span><span class="sxs-lookup"><span data-stu-id="f1f5c-108">Check if you are already pre-approved for invoice payment.</span></span>
- <span data-ttu-id="f1f5c-109">Laskun maksu on käytettävissä vain yritys tileillä, ei henkilökohtaisissa tileissä.</span><span class="sxs-lookup"><span data-stu-id="f1f5c-109">Invoice pay is only available for business accounts, not for personal accounts.</span></span>
- <span data-ttu-id="f1f5c-110">Sinun on maksettava kaikki erääntyneet maksut ennen laskun maksuun siirtymistä.</span><span class="sxs-lookup"><span data-stu-id="f1f5c-110">You must pay all outstanding charges before switching to invoice pay.</span></span>
- <span data-ttu-id="f1f5c-111">Tuki tiimi tarkistaa tilin määrittääkseen, onko se oikeutettu laskun maksu tilaan.</span><span class="sxs-lookup"><span data-stu-id="f1f5c-111">The support team will review the account to determine if it is eligible for invoice mode of payment.</span></span>
- <span data-ttu-id="f1f5c-112">Laskun maksu tapaa ei voi käyttää Marketplace 3rd Party-palveluissa; Jos aiot vaihtaa nykyisen tila uksen laskuun, joka sisältää Marketplace-tai 3rd party-palveluja, nämä palvelut on poistettava ennen vaihtamista.</span><span class="sxs-lookup"><span data-stu-id="f1f5c-112">Invoice mode of payment is not supported for marketplace 3rd party services; if you intend to switch a current subscription to an invoice that contains marketplace or 3rd party services, these services must be deleted before switching.</span></span> <span data-ttu-id="f1f5c-113">Jos kyseessä on tuleva Marketplace-palvelu, Osta ensin erillinen tilaus luotto kortilta ja Osta tai ota Marketplacen kolmannen osapuolen palvelut.</span><span class="sxs-lookup"><span data-stu-id="f1f5c-113">For future marketplace services, purchase a separate subscription on credit card first and then purchase or deploy marketplace 3rd party services.</span></span>
- <span data-ttu-id="f1f5c-114">Kun siirryt lasku maksuun, et voi siirtyä takaisin luotto-tai maksu kortti maksuun.</span><span class="sxs-lookup"><span data-stu-id="f1f5c-114">Once you switch to invoice pay, you can't switch back to credit or debit card payment.</span></span>

<span data-ttu-id="f1f5c-115">*Kun olet hyväksynyt maksu laskun*, voit vaihtaa Azure-tila uksen laskun maksetuksi sekillä tai pankki siirrolla  [Azure-portaalissa](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="f1f5c-115">*Once you're approved to pay by invoice*, you can switch your Azure subscription to the invoice pay via cheque or wire transfer in the [Azure portal](https://portal.azure.com/).</span></span>
<span data-ttu-id="f1f5c-116">Voit tehdä sen seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="f1f5c-116">To do that:</span></span>

1. <span data-ttu-id="f1f5c-117">Kirjaudu sisään Azure- [portaaliin](https://portal.azure.com/)   tilin järjestelmänvalvojana.</span><span class="sxs-lookup"><span data-stu-id="f1f5c-117">Sign in to the [Azure portal](https://portal.azure.com/) as the Account Administrator.</span></span> <span data-ttu-id="f1f5c-118">Hae ja valitse **kustannusten hallinta + laskutus**.</span><span class="sxs-lookup"><span data-stu-id="f1f5c-118">Search for and select **Cost Management + Billing**.</span></span>
2. <span data-ttu-id="f1f5c-119">Valitse tilaus, jonka haluat vaihtaa laskun maksuun.</span><span class="sxs-lookup"><span data-stu-id="f1f5c-119">Select the subscription you would like to switch to invoice payment.</span></span> <span data-ttu-id="f1f5c-120">Valitse **Maksu tavat**.</span><span class="sxs-lookup"><span data-stu-id="f1f5c-120">Select **Payment methods**.</span></span>
3. <span data-ttu-id="f1f5c-121">Napsauta komento palkissa **maksu laskulla** -painiketta.</span><span class="sxs-lookup"><span data-stu-id="f1f5c-121">In the command bar, click the **Pay by invoice** button.</span></span>

<span data-ttu-id="f1f5c-122">**Suositellut asia kirjat**</span><span class="sxs-lookup"><span data-stu-id="f1f5c-122">**Recommended Documents**</span></span>

- [<span data-ttu-id="f1f5c-123">Pyydä/Lataa/Näytä Azure-laskutus lasku ja käyttö tiedot</span><span class="sxs-lookup"><span data-stu-id="f1f5c-123">Request/Download/View your Azure billing invoice and usage data</span></span>](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date)
- [<span data-ttu-id="f1f5c-124">Azure-laskujen lähettäminen suoraan Saapuneet-kansioon</span><span class="sxs-lookup"><span data-stu-id="f1f5c-124">How to email Azure invoices directly to your inbox</span></span>](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date)
- [<span data-ttu-id="f1f5c-125">Maksaminen laskulla</span><span class="sxs-lookup"><span data-stu-id="f1f5c-125">Pay by invoice</span></span>](https://docs.microsoft.com/azure/billing/billing-how-to-pay-by-invoice)
- [<span data-ttu-id="f1f5c-126">Yksityiskohtaisten käyttö maksujen ymmärtäminen</span><span class="sxs-lookup"><span data-stu-id="f1f5c-126">Understand detailed usage charges</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-your-bill)
- [<span data-ttu-id="f1f5c-127">Laskun termien ymmärtäminen</span><span class="sxs-lookup"><span data-stu-id="f1f5c-127">Understand terms on your invoice</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-your-invoice)
- [<span data-ttu-id="f1f5c-128">Omistajuuden siirtäminen</span><span class="sxs-lookup"><span data-stu-id="f1f5c-128">How to transfer ownership</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer)
