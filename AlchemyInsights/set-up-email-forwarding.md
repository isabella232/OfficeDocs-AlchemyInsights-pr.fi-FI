---
title: Sähköpostin edelleenlähetysten määrittäminen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "20"
- "1200004"
ms.assetid: 15abf81d-5c5d-49da-ac81-1b4daa1809f6
ms.openlocfilehash: a7fba259375c667ff2e0f14a03972e102468cd27
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51787134"
---
# <a name="check-the-email-forwarding-settings-for-a-mailbox"></a><span data-ttu-id="9a383-102">Postilaatikon sähköpostin edelleenlähetysasetusten tarkastaminen</span><span class="sxs-lookup"><span data-stu-id="9a383-102">Check the email forwarding settings for a mailbox</span></span>

<span data-ttu-id="9a383-103">Ensinnäkin sähköpostin edelleenlähetys on otettava käyttöön vuokraajan tasolla.</span><span class="sxs-lookup"><span data-stu-id="9a383-103">Firstly, email forwarding has to be enabled on the tenant level.</span></span> <span data-ttu-id="9a383-104">Jos olet määrittänyt sähköpostin edelleenlähetystä postilaatikkoon, mutta se ei toimi (saat virheilmoituksen **"550 5.7.520 Käyttö estetty,** Organisaatiosi ei salli ulkoista edelleenlähetystä") on kohdassa Automaattisen ulkoisen sähköpostin edelleenlähetysten hallinta [Microsoft 365:ssä.](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="9a383-104">If you have set up email forwarding on a mailbox, but it is not working (you get an error **"550 5.7.520 Access denied, Your organization does not allow external forwarding"**) please see [Control automatic external email forwarding in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding?view=o365-worldwide).</span></span>

<span data-ttu-id="9a383-105">Postilaatikon sähköpostin edelleenlähetysasetukset on helppo vahvistaa.</span><span class="sxs-lookup"><span data-stu-id="9a383-105">It's easy to verify the email forwarding settings on a mailbox!</span></span> <span data-ttu-id="9a383-106">Noudata näitä ohjeita.</span><span class="sxs-lookup"><span data-stu-id="9a383-106">Just follow these steps.</span></span>
  
> <span data-ttu-id="9a383-107">Jos kyse on käyttäjän postilaatikosta, valitse **Käyttäjät,** jotka ovat aktiivisia käyttäjiä ja valitse käyttäjä, jonka \>  postilaatikon haluat lähettää edelleen.</span><span class="sxs-lookup"><span data-stu-id="9a383-107">If this is a user mailbox, go to **Users** \> **Active users** and select the user whose mailbox you're forwarding.</span></span> <span data-ttu-id="9a383-108">Valitse **Sähköposti-välilehdessä** **Sähköpostin edelleenlähetysten hallinta**.</span><span class="sxs-lookup"><span data-stu-id="9a383-108">On the **Mail** tab, select **Manage email forwarding**.</span></span>

> <span data-ttu-id="9a383-109">Jos tämä on jaettu postilaatikko, siirry **ryhmät** \> **jaettuihin postilaatikoihin** ja valitse jaettu postilaatikko, jonka haluat lähettää edelleen.</span><span class="sxs-lookup"><span data-stu-id="9a383-109">If this is a shared mailbox, go to **Groups** \> **Shared mailboxes** and select the shared mailbox you're forwarding.</span></span> <span data-ttu-id="9a383-110">Valitse **Muokkaa sähköpostin** edelleenlähetystä varten.</span><span class="sxs-lookup"><span data-stu-id="9a383-110">Select **Edit** for email forwarding.</span></span>

<span data-ttu-id="9a383-111">Lisätietoja on kohdassa Sähköpostin [edelleenlähetysten määrittäminen Microsoft 365:ssä.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)</span><span class="sxs-lookup"><span data-stu-id="9a383-111">For more information, see [Configure email forwarding in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>
  
<span data-ttu-id="9a383-112">Jos haluat lähettää käyttäjille ohjeet, jotta he voivat määrittää sähköpostin edelleen lähettämisen omiin postilaatikoihinsa, osoita heitä kohtaan Sähköpostin lähettäminen [edelleen Microsoft 365:stä toiseen sähköpostitiliin](https://support.office.com/article/Forward-email-from-Office-365-to-another-email-account-1ed4ee1e-74f8-4f53-a174-86b748ff6a0e).</span><span class="sxs-lookup"><span data-stu-id="9a383-112">To send instructions to your users so they can set up email forwarding on their own mailboxes, point them to [Forward email from Microsoft 365 to another email account](https://support.office.com/article/Forward-email-from-Office-365-to-another-email-account-1ed4ee1e-74f8-4f53-a174-86b748ff6a0e).</span></span> <span data-ttu-id="9a383-113">Huomaa, että voit lähettää viestin edelleen vain yhteen sähköpostiosoitteeseen.</span><span class="sxs-lookup"><span data-stu-id="9a383-113">Please note that you can forward to only one email address.</span></span> <span data-ttu-id="9a383-114">Jos haluat määrittää edelleenlähetystä henkilöryhmälle, luo jakeluluettelo (Ryhmät-kohdassa), lisää käyttäjät siihen ja määritä sitten edelleenlähetys tähän ryhmään.</span><span class="sxs-lookup"><span data-stu-id="9a383-114">If you need to set up forwarding to a group of people, create a distribution list (under **Groups**), add your users to it, and then configure forwarding to that group.</span></span>
  
<span data-ttu-id="9a383-115">Onko työntekijä jättämässä tietoja?</span><span class="sxs-lookup"><span data-stu-id="9a383-115">Do you have an employee leaving?</span></span> <span data-ttu-id="9a383-116">Katso suositellut ohjeet ohjeista entisen työntekijän poistaminen [Microsoft 365:stä.](https://docs.microsoft.com/microsoft-365/admin/add-users/remove-former-employee)</span><span class="sxs-lookup"><span data-stu-id="9a383-116">See [Remove a former employee from Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/remove-former-employee) for the recommended steps.</span></span>