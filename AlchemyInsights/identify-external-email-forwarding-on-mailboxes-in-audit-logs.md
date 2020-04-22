---
title: Postilaatikoiden ulkoisen sähköpostin edelleenlähetyksen tunnistaminen valvontalokeissa
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
ms.openlocfilehash: 156fd0044cdc42230ace0a5db16f49af572bb6fa
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716457"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="af88c-102">Tunnista, milloin ulkoinen sähköpostin edelleenlähetys on määritetty postilaatikoissa</span><span class="sxs-lookup"><span data-stu-id="af88c-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="af88c-103">Kun Microsoft 365 -käyttäjä määrittää postilaatikon ulkoisen sähköpostin edelleenlähetyksen, aktiviteettia valvotaan osana **Set-Mailbox-cmdlet-tiedostoa.**</span><span class="sxs-lookup"><span data-stu-id="af88c-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="af88c-104">Toiminta näkyy valvontalokihaun avulla Suojaus-& yhteensopivuuskeskuksessa.</span><span class="sxs-lookup"><span data-stu-id="af88c-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="af88c-105">Kirjaudu Microsoft [365 Security & Compliance Centeriin.](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="af88c-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="af88c-106">Siirry **Haun** > **valvontalokin hakusivulle.**</span><span class="sxs-lookup"><span data-stu-id="af88c-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="af88c-107">Valitse päivämääräväli **Aloituspäivä-** ja **Päättymispäivä-kentissä.**</span><span class="sxs-lookup"><span data-stu-id="af88c-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="af88c-108">Käyttäjänimeä ei tarvitse määrittää.</span><span class="sxs-lookup"><span data-stu-id="af88c-108">You don't need to specify a username.</span></span> <span data-ttu-id="af88c-109">Tarkista, että **Aktiviteetit-kentän** arvo on **Näytä kaikkien aktiviteettien tulokset**.</span><span class="sxs-lookup"><span data-stu-id="af88c-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="af88c-110">Valitse **Hae**.</span><span class="sxs-lookup"><span data-stu-id="af88c-110">Click **Search**.</span></span>

<span data-ttu-id="af88c-111">Valitse tuloksista **Suodata tulokset** ja kirjoita aktiviteettisuodatinruutuun **Set-Mailbox.**</span><span class="sxs-lookup"><span data-stu-id="af88c-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="af88c-112">Valitse tuloksista valvontatietue.</span><span class="sxs-lookup"><span data-stu-id="af88c-112">Select an audit record in the results.</span></span> <span data-ttu-id="af88c-113">Valitse **Tiedot-pikaikkunassa** **Lisätietoja**.</span><span class="sxs-lookup"><span data-stu-id="af88c-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="af88c-114">Sinun on tarkasteltava kunkin valvontatietueen tietoja selvittääksesi, liittyykö aktiviteetti sähköpostin edelleenlähettämiseen.</span><span class="sxs-lookup"><span data-stu-id="af88c-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="af88c-115">**ObjectId**: Muokatun postilaatikon aliasarvo.</span><span class="sxs-lookup"><span data-stu-id="af88c-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="af88c-116">**Parametrit**: _ForwardingSmtpAddress_ ilmaisee kohdesähköpostiosoitteen.</span><span class="sxs-lookup"><span data-stu-id="af88c-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="af88c-117">**UserId**: Käyttäjä, joka on määrittänyt sähköpostin edelleenlähetyksen postilaatikkoon **ObjectId-kentässä.**</span><span class="sxs-lookup"><span data-stu-id="af88c-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="af88c-118">Lisätietoja on ohjeaiheessa [Postilaatikon sähköpostin edelleenlähetyksen määrittäminen](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="af88c-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
