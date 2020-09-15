---
title: Valvonta lokien posti laatikoiden ulkoinen sähkö postin lähettäminen edelleen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696294"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="58d84-102">Määritä, milloin ulkoinen sähkö postin välitys on määritetty posti laatikoihin</span><span class="sxs-lookup"><span data-stu-id="58d84-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="58d84-103">Kun Microsoft 365-käyttäjä määrittää posti laatikon ulkoiseen sähkö postin lähettämiseen, toiminta tarkastetaan osana **joukko posti laatikon cmdlet-** komentosovelmaa.</span><span class="sxs-lookup"><span data-stu-id="58d84-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="58d84-104">Voit tarkastella aktiviteettia valvonta loki haun avulla tieto turva-& yhteensopivuus keskuksessa.</span><span class="sxs-lookup"><span data-stu-id="58d84-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="58d84-105">Kirjaudu sisään [Microsoft 365-tieto turva & Compliance Centeriin](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="58d84-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="58d84-106">Siirry **haun**  >  **valvonta lokien haku** sivulle.</span><span class="sxs-lookup"><span data-stu-id="58d84-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="58d84-107">Valitse päivämäärä väli **alkamis päivä** -ja **päättymis päivä** -kenttiin.</span><span class="sxs-lookup"><span data-stu-id="58d84-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="58d84-108">Sinun ei tarvitse määrittää käyttäjä nimeä.</span><span class="sxs-lookup"><span data-stu-id="58d84-108">You don't need to specify a username.</span></span> <span data-ttu-id="58d84-109">Varmista, että **aktiviteetit** -kenttä on valittu **näyttämään kaikkien toimintojen tulokset**.</span><span class="sxs-lookup"><span data-stu-id="58d84-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="58d84-110">Valitse **Hae**.</span><span class="sxs-lookup"><span data-stu-id="58d84-110">Click **Search**.</span></span>

<span data-ttu-id="58d84-111">Valitse tulokset-kohdassa **Suodata tulokset** ja kirjoita **Määritä-posti laatikko** aktiviteetin suodatus-ruutuun.</span><span class="sxs-lookup"><span data-stu-id="58d84-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="58d84-112">Valitse seuranta tietue tuloksista.</span><span class="sxs-lookup"><span data-stu-id="58d84-112">Select an audit record in the results.</span></span> <span data-ttu-id="58d84-113">Valitse **tiedot** -valikosta **lisä tietoja**.</span><span class="sxs-lookup"><span data-stu-id="58d84-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="58d84-114">Sinun on tarkasteltava kunkin valvonta tietueen tietoja määrittääksesi, onko toiminto yhteydessä sähkö postin lähettämiseen.</span><span class="sxs-lookup"><span data-stu-id="58d84-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="58d84-115">**ObjectID**: muutetun posti laatikon alias-arvo.</span><span class="sxs-lookup"><span data-stu-id="58d84-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="58d84-116">**Parametrit**: _fordingingsmtpaddress_ osoittaa kohde Sähkö posti osoitteen.</span><span class="sxs-lookup"><span data-stu-id="58d84-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="58d84-117">**UserID**: käyttäjä, joka määritti sähkö postin lähettämisen **objectID** -kentässä olevalle posti laatikolle.</span><span class="sxs-lookup"><span data-stu-id="58d84-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="58d84-118">Lisä tietoja [on kohdassa sähkö postin lähettämisen määrittäminen Posti laatikolle](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="58d84-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
