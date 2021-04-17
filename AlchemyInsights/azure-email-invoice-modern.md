---
title: Moderni Azure-sähköpostilasku
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820823"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="14b48-102">Sähköpostilaskutus Azuressa</span><span class="sxs-lookup"><span data-stu-id="14b48-102">Email invoicing in Azure</span></span>

<span data-ttu-id="14b48-103">Sinulla on oltava laskutusprofiilin tai laskutustilin omistajan tai osallistujan rooli, jotta voit päivittää sähköpostilaskutusasetuksia.</span><span class="sxs-lookup"><span data-stu-id="14b48-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="14b48-104">Kun olet ottanut ominaisuuden käyttöön, kaikki käyttäjät, joilla on laskutusprofiilin omistajan, osallistujan, lukijan tai laskutusvastaavan rooli, saavat laskun sähköpostiinsa.</span><span class="sxs-lookup"><span data-stu-id="14b48-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="14b48-105">Kirjaudu [Azure-portaaliin](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="14b48-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="14b48-106">Etsi **Kustannustenhallinta ja laskutus**.</span><span class="sxs-lookup"><span data-stu-id="14b48-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="14b48-107">Valitse vasemmasta reunasta **Laskut** ja valitse sitten sivun yläreunasta **Sähköpostilasku**.</span><span class="sxs-lookup"><span data-stu-id="14b48-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="14b48-108">Jos sinulla on useita laskutusprofiileja, valitse ensin laskutusprofiili ja sitten **Ota käyttöön**.</span><span class="sxs-lookup"><span data-stu-id="14b48-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="14b48-109">Valitse **Päivitä**.</span><span class="sxs-lookup"><span data-stu-id="14b48-109">Select **Update**.</span></span>
6. <span data-ttu-id="14b48-110">Jos sinulla on useita laskutusprofiileja, valitse ensin laskutusprofiili ja sitten **Ota käyttöön**.</span><span class="sxs-lookup"><span data-stu-id="14b48-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="14b48-111">Voit antaa muille oikeuden tarkastella, ladata ja maksaa laskuja määrittämällä heille MCA- tai MPA-laskutusprofiilin laskutusvastaavan roolin.</span><span class="sxs-lookup"><span data-stu-id="14b48-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="14b48-112">Jos olet ottanut sähköpostilaskut käyttöön, käyttäjät saavat myös laskut sähköpostitse.</span><span class="sxs-lookup"><span data-stu-id="14b48-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="14b48-113">Kirjaudu [Azure-portaaliin](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="14b48-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="14b48-114">Etsi **Kustannustenhallinta ja laskutus**.</span><span class="sxs-lookup"><span data-stu-id="14b48-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="14b48-115">Valitse vasemmasta reunasta **Laskutusprofiilit**.</span><span class="sxs-lookup"><span data-stu-id="14b48-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="14b48-116">Valitse laskutusprofiilien luettelosta profiili, jolle haluat määrittää laskutusvastaavan roolin.</span><span class="sxs-lookup"><span data-stu-id="14b48-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="14b48-117">Valitse vasemmasta reunasta **Käyttöoikeuksien valvonta** ja valitse sitten sivun yläreunasta **Lisää**.</span><span class="sxs-lookup"><span data-stu-id="14b48-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="14b48-118">Valitse avattavasta Rooli-luettelosta **Laskutusvastaava**.</span><span class="sxs-lookup"><span data-stu-id="14b48-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="14b48-119">Myönnä käyttöoikeus kirjoittamalla käyttäjän sähköpostiosoite.</span><span class="sxs-lookup"><span data-stu-id="14b48-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="14b48-120">Määritä rooli valitsemalla **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="14b48-120">Select **Save** to assign the role.</span></span>
