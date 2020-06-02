---
title: Ulkoisen sähköpostin edelleenlähetyksen tunnistaminen valvontalokeissa
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 592eb92e4b0fe0f9da2fa20bb93ffa4fbbb76662
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508949"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="5d348-102">Ulkoisen sähköpostin edelleenlähetyksen määrittäminen postilaatikoissa</span><span class="sxs-lookup"><span data-stu-id="5d348-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="5d348-103">Kun Microsoft 365 -käyttäjä määrittää postilaatikon ulkoisen sähköpostin edelleenlähetyksen, aktiviteettia valvotaan osana **Set-Mailbox-cmdlet-komentoa.**</span><span class="sxs-lookup"><span data-stu-id="5d348-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="5d348-104">Voit tarkastella toimintaa valvontalokin haun avulla Suojaus- & Yhteensopivuuskeskuksessa.</span><span class="sxs-lookup"><span data-stu-id="5d348-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="5d348-105">Kirjaudu Microsoft [365 Security & Compliance Centeriin.](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="5d348-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="5d348-106">Siirry **Haun**  >  **valvontalokin hakusivulle.**</span><span class="sxs-lookup"><span data-stu-id="5d348-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="5d348-107">Valitse päivämääräalue **Aloituspäivä-** ja **Päättymispäivä-kentissä.**</span><span class="sxs-lookup"><span data-stu-id="5d348-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="5d348-108">Käyttäjänimeä ei tarvitse määrittää.</span><span class="sxs-lookup"><span data-stu-id="5d348-108">You don't need to specify a username.</span></span> <span data-ttu-id="5d348-109">Tarkista, että **Aktiviteetit-kentän** arvoksi on määritetty **Näytä kaikkien aktiviteettien tulokset**.</span><span class="sxs-lookup"><span data-stu-id="5d348-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="5d348-110">Valitse **Hae**.</span><span class="sxs-lookup"><span data-stu-id="5d348-110">Click **Search**.</span></span>

<span data-ttu-id="5d348-111">Valitse tuloksista **Suodata tulokset** ja kirjoita aktiviteettisuodatinruutuun **Set-Mailbox.**</span><span class="sxs-lookup"><span data-stu-id="5d348-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="5d348-112">Valitse seurantatietue tuloksista.</span><span class="sxs-lookup"><span data-stu-id="5d348-112">Select an audit record in the results.</span></span> <span data-ttu-id="5d348-113">Valitse **Details** Tiedot-pikaikkunassa **Lisätietoja**.</span><span class="sxs-lookup"><span data-stu-id="5d348-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="5d348-114">Sinun on tarkasteltava kunkin valvontatietueen tietoja ja määritettävä, liittyykö aktiviteetti sähköpostin edelleenlähetykseen.</span><span class="sxs-lookup"><span data-stu-id="5d348-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="5d348-115">**ObjectId**: Muokattavan postilaatikon aliasarvo.</span><span class="sxs-lookup"><span data-stu-id="5d348-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="5d348-116">**Parametrit**: _ForwardingSmtpAddress_ ilmaisee kohdesähköpostiosoitteen.</span><span class="sxs-lookup"><span data-stu-id="5d348-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="5d348-117">**UserId**: Käyttäjä, joka on määrittänyt sähköpostin edelleenlähetyksen **postilaatikkoon ObjectId-kentässä.**</span><span class="sxs-lookup"><span data-stu-id="5d348-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="5d348-118">Lisätietoja on [ohjeaiheessa Postilaatikon sähköpostin edelleenlähetyksen määrittäminen](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="5d348-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
