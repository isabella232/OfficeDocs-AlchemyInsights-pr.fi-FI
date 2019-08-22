---
title: Määritä ulkoisen sähköpostin välityksen seurantalokeja postilaatikoita
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7defd0902e8c8bebae9c7bfee72c3199cbc1909f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539098"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="03b8a-102">Tunnistaa, kun postilaatikoita ulkoisen sähköpostin edelleenlähetys on määritetty</span><span class="sxs-lookup"><span data-stu-id="03b8a-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="03b8a-103">Kun Office 365-käyttäjä määrittää postilaatikkoon ulkoisen sähköpostin edelleenlähetys, toimintaa tarkistetaan osana **Set-Mailbox** -cmdlet-komennolla.</span><span class="sxs-lookup"><span data-stu-id="03b8a-103">When an Office 365  user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="03b8a-104">Voit tarkastella tehtävän tarkastuksen lokista etsintää käyttämällä suojauksen & Compliance Centeriin.</span><span class="sxs-lookup"><span data-stu-id="03b8a-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="03b8a-105">Kirjautua sisään [Office 365 & noudattamista Tietoturvakeskus](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="03b8a-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="03b8a-106">Siirry **Etsinnän** > **Audit log** etsintäsivun.</span><span class="sxs-lookup"><span data-stu-id="03b8a-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="03b8a-107">Valitse **aloituspäivä** - ja **päättymispäivä** -kenttiin päivämääräalue.</span><span class="sxs-lookup"><span data-stu-id="03b8a-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="03b8a-108">Sinun ei tarvitse määrittää käyttäjänimi.</span><span class="sxs-lookup"><span data-stu-id="03b8a-108">You don't need to specify a username.</span></span> <span data-ttu-id="03b8a-109">Tarkista tulokset **kaikista** **aktiviteetit** -kentässä on määritetty.</span><span class="sxs-lookup"><span data-stu-id="03b8a-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="03b8a-110">Valitse **Etsi**.</span><span class="sxs-lookup"><span data-stu-id="03b8a-110">Click **Search**.</span></span>

<span data-ttu-id="03b8a-111">**Suodatuksen tulokset** valitsemalla tulokset ja kirjoita Suodata-ruutuun aktiviteetin **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="03b8a-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="03b8a-112">Valitse tuloksia koskeva seurantatietue.</span><span class="sxs-lookup"><span data-stu-id="03b8a-112">Select an audit record in the results.</span></span> <span data-ttu-id="03b8a-113">Valitse **tiedot** -valikon avauspainike **Lisätietoja**.</span><span class="sxs-lookup"><span data-stu-id="03b8a-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="03b8a-114">On tarkasteltavan määrittääkseen, jos tehtävä liittyy sähköpostin edelleenlähetys kunkin valvontatietueen tietojen.</span><span class="sxs-lookup"><span data-stu-id="03b8a-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="03b8a-115">**ObjectId**: tunnuksen arvo postilaatikko, johon tehtiin muutoksia.</span><span class="sxs-lookup"><span data-stu-id="03b8a-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="03b8a-116">**Parametrit**: _ForwardingSmtpAddress_ ilmaisee kohteen sähköpostiosoite.</span><span class="sxs-lookup"><span data-stu-id="03b8a-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="03b8a-117">**Käyttäjätunnus**: käyttäjä, joka on määritetty sähköpostin edelleenlähetys postilaatikon **ObjectId** -kentässä.</span><span class="sxs-lookup"><span data-stu-id="03b8a-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="03b8a-118">Lisätietoja [määrittäminen, joka määrittää sähköpostiviestin välittäminen postilaatikkoon](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="03b8a-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
