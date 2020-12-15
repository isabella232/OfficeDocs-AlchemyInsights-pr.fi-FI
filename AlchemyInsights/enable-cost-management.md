---
title: Ota kustannusten hallinta käyttöön
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677220"
---
# <a name="enable-cost-management"></a><span data-ttu-id="51ca9-102">Ota kustannusten hallinta käyttöön</span><span class="sxs-lookup"><span data-stu-id="51ca9-102">Enable cost management</span></span>

<span data-ttu-id="51ca9-103">**Mitä kuluja organisaation käytöstä poistetut kustannukset tarkoittavat?**</span><span class="sxs-lookup"><span data-stu-id="51ca9-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="51ca9-104">Enterprise Agreement (EA)-tai Microsoftin asiakas sopimus (MCA)-tileillä käyttävät organisaatiot voivat estää kustannus tietojen ja hinta tietojen käytön.</span><span class="sxs-lookup"><span data-stu-id="51ca9-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="51ca9-105">Kun olet kirjautunut sisään Azure-portaaliin, hän voi käyttää laskutuksen ohjelmointi raja pintoja ja hakea ohjelmallisesti laskuja (kun olet ottanut käyttöön) ja käyttö tietoja.</span><span class="sxs-lookup"><span data-stu-id="51ca9-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="51ca9-106">**Laskujen käyttö oikeuksien salliminen muille käyttäjille**</span><span class="sxs-lookup"><span data-stu-id="51ca9-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="51ca9-107">Siirry paketit- **terään** Azure-portaalissa.</span><span class="sxs-lookup"><span data-stu-id="51ca9-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="51ca9-108">Valitse **laskut** ja sitten **laskujen käyttäminen**.</span><span class="sxs-lookup"><span data-stu-id="51ca9-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="51ca9-109">Ota käyttö oikeus käyttöön ja tallenna sitten muutokset, jotta käyttäjät voivat tilata tila uksen-rajatut roolit laskujen lataamista varten.</span><span class="sxs-lookup"><span data-stu-id="51ca9-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="51ca9-110">Tilin hallinnoija voi myös määrittää, että laskut lähetetään sähköpostitse.</span><span class="sxs-lookup"><span data-stu-id="51ca9-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="51ca9-111">Lisä tietoja on artikkelissa [laskun saaminen sähköpostitse](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span><span class="sxs-lookup"><span data-stu-id="51ca9-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="51ca9-112">**Käyttäjien lisääminen laskutuksen luku ohjelman rooliin**</span><span class="sxs-lookup"><span data-stu-id="51ca9-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="51ca9-113">Siirry paketit- **terään** Azure-portaalissa.</span><span class="sxs-lookup"><span data-stu-id="51ca9-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="51ca9-114">Valitse **käytön hallinta (IAM)** ja valitse sitten **Lisää**.</span><span class="sxs-lookup"><span data-stu-id="51ca9-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="51ca9-115">Valitse **Valitse rooli** -sivulla **laskutuksen luku ohjelma** .</span><span class="sxs-lookup"><span data-stu-id="51ca9-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="51ca9-116">Kirjoita kutsuttavan käyttäjän Sähkö posti viesti ja Lähetä kutsu valitsemalla **OK** .</span><span class="sxs-lookup"><span data-stu-id="51ca9-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="51ca9-117">Noudata kutsu Sähkö posti viestissä annettuja ohjeita, jotta voit kirja utua sisään laskutuslukijana.</span><span class="sxs-lookup"><span data-stu-id="51ca9-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="51ca9-118">Lisä tietoja on kohdassa [laskutuksen käytön myöntäminen](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span><span class="sxs-lookup"><span data-stu-id="51ca9-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="51ca9-119">**Suositellut asia kirjat**</span><span class="sxs-lookup"><span data-stu-id="51ca9-119">**Recommended documents**</span></span>

- [<span data-ttu-id="51ca9-120">Ota käyttöön DA-ja AO-näkymät EA-portaalin kautta</span><span class="sxs-lookup"><span data-stu-id="51ca9-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="51ca9-121">Kustannusten hallintaan sisältyvät kustannukset</span><span class="sxs-lookup"><span data-stu-id="51ca9-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="51ca9-122">Tuetuissa Microsoft Azure-Tarjoissa</span><span class="sxs-lookup"><span data-stu-id="51ca9-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="51ca9-123">Kustannus analyysin kustannusten tarkasteleminen</span><span class="sxs-lookup"><span data-stu-id="51ca9-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="51ca9-124">Laskutus tietojen käytön tarjoaminen</span><span class="sxs-lookup"><span data-stu-id="51ca9-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="51ca9-125">Microsoft-asiakas sopimuksen käytön tarkistaminen</span><span class="sxs-lookup"><span data-stu-id="51ca9-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






