---
title: Useilla objekteilla on sama sähköpostiosoite kuin henkilöllisyydellä
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438930"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="9237e-102">Useilla objekteilla on sama sähköpostiosoite kuin henkilöllisyydellä</span><span class="sxs-lookup"><span data-stu-id="9237e-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="9237e-103">**Useita objekteja**</span><span class="sxs-lookup"><span data-stu-id="9237e-103">**Multiple objects**</span></span>

<span data-ttu-id="9237e-104">Yksi tämän virheen yleisistä syistä ei ole se, että Outlook Web Access -pyyntöä ei voi reitittää oikein, jos useissa objekteissa on sama sähköpostiosoite kuin käyttäjätiteetillä.</span><span class="sxs-lookup"><span data-stu-id="9237e-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="9237e-105">Voit etsiä nämä objektit suorittamalla seuraavat komennot:</span><span class="sxs-lookup"><span data-stu-id="9237e-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="9237e-106">· Get-Vastaanottaja<email address></span><span class="sxs-lookup"><span data-stu-id="9237e-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="9237e-107">· Get-Käyttäjä<email address></span><span class="sxs-lookup"><span data-stu-id="9237e-107">· Get-User <email address></span></span>

<span data-ttu-id="9237e-108">· Get-User <email address> -SoftDeletedUser (Get-User -SoftDeletedUser)</span><span class="sxs-lookup"><span data-stu-id="9237e-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="9237e-109">· Ota yhteyttä<email address></span><span class="sxs-lookup"><span data-stu-id="9237e-109">· Get-Contact <email address></span></span>

<span data-ttu-id="9237e-110">· Get-Postilaatikko <email address> -PublicFolder</span><span class="sxs-lookup"><span data-stu-id="9237e-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="9237e-111">· Get-Postilaatikko <email address> -IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="9237e-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="9237e-112">· Get-Postilaatikko <email address> -InactiveMailboxVain</span><span class="sxs-lookup"><span data-stu-id="9237e-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="9237e-113">Voit ratkaista ongelman poistamalla useita objekteja, joilla on sama sähköposti-identiteetti, ja varmistamalla, että on olemassa yksi objekti, jolla on tietty sähköpostitunniste ja että sen vastaanottajatyyppi on UserMailbox.</span><span class="sxs-lookup"><span data-stu-id="9237e-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="9237e-114">**Samaa osoitetta käytetään yritys- ja kuluttajapostilaatikoissa**</span><span class="sxs-lookup"><span data-stu-id="9237e-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="9237e-115">Toinen syy on se, että samaa osoitetta käytetään yritys- ja kuluttajapostilaatikoissa.</span><span class="sxs-lookup"><span data-stu-id="9237e-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="9237e-116">Tässä tapauksessa käyttäjän on muutettava ensisijaista kuluttajaaliastaan, kunnes Cafe tukee tätä skenaariota.</span><span class="sxs-lookup"><span data-stu-id="9237e-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="9237e-117">Tämä on pysyvä virhe, joka ei katoa ilman väliintuloa.</span><span class="sxs-lookup"><span data-stu-id="9237e-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="9237e-118">Lisätietoja on [ohjeaiheessa Microsoft-tilin sähköpostiosoitteen tai puhelinnumeron muuttaminen](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="9237e-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>