---
title: Määritä ulkoisen sähköpostin välityksen seurantalokeja postilaatikoita
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 7fb2c161c558a7eb961f86ca2b86e33750d902fd
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32417209"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="5053d-102">Tunnistaa, kun postilaatikoita ulkoisen sähköpostin edelleenlähetys on määritetty</span><span class="sxs-lookup"><span data-stu-id="5053d-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="5053d-103">Kun käyttäjä määrittää postilaatikkoon ulkoisen sähköpostin edelleenlähetys, toimintaa tarkistetaan osana **Set-Mailbox** -cmdlet-komennolla.</span><span class="sxs-lookup"><span data-stu-id="5053d-103">When a user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="5053d-104">Voit tarkastella tehtävän tarkastuksen lokista etsintää käyttämällä suojauksen & Compliance Centeriin.</span><span class="sxs-lookup"><span data-stu-id="5053d-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="5053d-105">Kirjautua [Office 365-suojauksen & Compliance Centeriin](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="5053d-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="5053d-106">**Etsi ja tutkimus** ja valitse **Valvo lokista etsintää**.</span><span class="sxs-lookup"><span data-stu-id="5053d-106">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="5053d-107">Valitse **aloituspäivä** - ja **päättymispäivä** -kenttiin päivämääräalue.</span><span class="sxs-lookup"><span data-stu-id="5053d-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="5053d-108">Sinun ei tarvitse määrittää käyttäjänimi.</span><span class="sxs-lookup"><span data-stu-id="5053d-108">You don't need to specify a username.</span></span> <span data-ttu-id="5053d-109">Tarkista tulokset **kaikista** **aktiviteetit** -kentässä on määritetty.</span><span class="sxs-lookup"><span data-stu-id="5053d-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="5053d-110">Valitse **Etsi**.</span><span class="sxs-lookup"><span data-stu-id="5053d-110">Click **Search**.</span></span>

<span data-ttu-id="5053d-111">**Suodatuksen tulokset** valitsemalla tulokset ja kirjoita Suodata-ruutuun aktiviteetin **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="5053d-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="5053d-112">Valitse tuloksia koskeva seurantatietue.</span><span class="sxs-lookup"><span data-stu-id="5053d-112">Select an audit record in the results.</span></span> <span data-ttu-id="5053d-113">Valitse **tiedot** -valikon avauspainike **Lisätietoja**.</span><span class="sxs-lookup"><span data-stu-id="5053d-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="5053d-114">On tarkasteltavan määrittääkseen, jos tehtävä liittyy sähköpostin edelleenlähetys kunkin valvontatietueen tietojen.</span><span class="sxs-lookup"><span data-stu-id="5053d-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="5053d-115">**ObjectId**: tunnuksen arvo postilaatikko, johon tehtiin muutoksia.</span><span class="sxs-lookup"><span data-stu-id="5053d-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="5053d-116">**Parametrit**: _ForwardingSmtpAddress_ ilmaisee kohteen sähköpostiosoite.</span><span class="sxs-lookup"><span data-stu-id="5053d-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="5053d-117">**Käyttäjätunnus**: käyttäjä, joka on määritetty sähköpostin edelleenlähetys postilaatikon **ObjectId** -kentässä.</span><span class="sxs-lookup"><span data-stu-id="5053d-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="5053d-118">Lisätietoja [määrittäminen, joka määrittää sähköpostiviestin välittäminen postilaatikkoon](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="5053d-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
