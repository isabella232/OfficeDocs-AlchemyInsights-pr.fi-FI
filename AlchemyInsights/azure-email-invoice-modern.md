---
title: Moderni Azure-Sähkö posti laskutus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 65df6091a97d4937379ded384a78b5d07aa76e42
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922059"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="601f2-102">Sähkö postin laskutus Azuressa</span><span class="sxs-lookup"><span data-stu-id="601f2-102">Email invoicing in Azure</span></span>

<span data-ttu-id="601f2-103">Sinulla on oltava omistajan tai osallistujan rooli laskutus profiilissa tai sen laskutus tilillä, jotta voit päivittää Sähkö posti laskun asetuksen.</span><span class="sxs-lookup"><span data-stu-id="601f2-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="601f2-104">Kun olet valinnut-kohdan, Kaikki käyttäjät, joilla on laskutus profiilissa omistaja, avustaja, lukija ja laskun hallinnan rooli, saavat laskunsa sähköpostitse.</span><span class="sxs-lookup"><span data-stu-id="601f2-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="601f2-105">Kirjaudu sisään Azure- [portaaliin](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="601f2-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="601f2-106">Hae **kustannusten hallinta + laskutus**.</span><span class="sxs-lookup"><span data-stu-id="601f2-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="601f2-107">Valitse **laskut** vasemmalta puolelta ja valitse sitten sivun yläreunasta **Sähkö posti lasku** .</span><span class="sxs-lookup"><span data-stu-id="601f2-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="601f2-108">Jos sinulla on useita laskutus profiileja, valitse Laskutus profiili ja valitse sitten **Ilmoittaudu**.</span><span class="sxs-lookup"><span data-stu-id="601f2-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="601f2-109">Valitse **Päivitä**.</span><span class="sxs-lookup"><span data-stu-id="601f2-109">Select **Update**.</span></span>
6. <span data-ttu-id="601f2-110">Jos sinulla on useita laskutus profiileja, valitse Laskutus profiili ja valitse sitten **Ilmoittaudu**.</span><span class="sxs-lookup"><span data-stu-id="601f2-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="601f2-111">Voit antaa muille käyttäjille oikeuden tarkastella, ladata ja maksaa laskuja määrittämällä heille MCA-tai MPA-laskutus profiilin laskun hallinnan roolin.</span><span class="sxs-lookup"><span data-stu-id="601f2-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="601f2-112">Jos olet valinnut, että saat laskun sähköpostitse, käyttäjät saavat laskut myös sähköpostitse.</span><span class="sxs-lookup"><span data-stu-id="601f2-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="601f2-113">Kirjaudu sisään Azure- [portaaliin](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="601f2-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="601f2-114">Hae **kustannusten hallinta + laskutus**.</span><span class="sxs-lookup"><span data-stu-id="601f2-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="601f2-115">Valitse **laskutus profiilit** vasemmalta puolelta.</span><span class="sxs-lookup"><span data-stu-id="601f2-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="601f2-116">Valitse Laskutus profiilit-luettelosta laskutus profiili, jolle haluat määrittää laskun hallinnan roolin.</span><span class="sxs-lookup"><span data-stu-id="601f2-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="601f2-117">Valitse vasemmasta reunasta **käytön hallinta (IAM)** ja valitse sitten **Lisää** sivun yläreunasta.</span><span class="sxs-lookup"><span data-stu-id="601f2-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="601f2-118">Valitse avattavasta rooli-luettelosta **laskun vastuu** henkilö.</span><span class="sxs-lookup"><span data-stu-id="601f2-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="601f2-119">Kirjoita sen käyttäjän Sähkö posti osoite, jolle haluat myöntää käyttö oikeuden.</span><span class="sxs-lookup"><span data-stu-id="601f2-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="601f2-120">Määritä rooli valitsemalla **Tallenna** .</span><span class="sxs-lookup"><span data-stu-id="601f2-120">Select **Save** to assign the role.</span></span>
