---
title: Poista viestitapahtumat valvontalokeissa
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 641c0216491186aeb423a13854c6b39ee005e5df
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508985"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="40963-102">Poistettujen sähköpostiviestien lokien valvonta</span><span class="sxs-lookup"><span data-stu-id="40963-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="40963-103">Microsoft on oletusarvoisesti ottanut postilaatikoiden valvontalokin käyttöön tammikuusta 2019 alkaen.</span><span class="sxs-lookup"><span data-stu-id="40963-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="40963-104">Muussa tapauksessa voit tarkastella tietyn käyttäjän poista viestitapahtumia manuaalisesti, jotta poistotoiminnot voidaan ottaa käyttöön manuaalisesti valvontaa varten.</span><span class="sxs-lookup"><span data-stu-id="40963-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="40963-105">Jos postilaatikon valvontaloki on jo otettu käyttöön organisaatiossasi tai tietylle käyttäjälle, noudata seuraavia ohjeita.</span><span class="sxs-lookup"><span data-stu-id="40963-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="40963-106">Kirjautuminen [Microsoft 365 Security & Compliance Centeriin](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="40963-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="40963-107">Valitse **Haku ja tutkinta** ja valitse **Valvontalokin haku**.</span><span class="sxs-lookup"><span data-stu-id="40963-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="40963-108">Valitse päivämääräalue **Aloituspäivä-** ja **Päättymispäivä-kentissä.**</span><span class="sxs-lookup"><span data-stu-id="40963-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="40963-109">Määritä käyttäjälle käyttäjänimi, jota haluat tutkia (käyttäjä, joka on poistanut kohteet).</span><span class="sxs-lookup"><span data-stu-id="40963-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="40963-110">Valitse **Aktiviteetit-kentässä** **Poistetut viestit Poistetut-kansiosta** ja **Siirretty viestit Poistetut-kansioon**.</span><span class="sxs-lookup"><span data-stu-id="40963-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="40963-111">Valitse **Hae**.</span><span class="sxs-lookup"><span data-stu-id="40963-111">Click **Search**.</span></span>

<span data-ttu-id="40963-112">Valitse tuloksista valvontatietue.</span><span class="sxs-lookup"><span data-stu-id="40963-112">In the results, select an audit record.</span></span> <span data-ttu-id="40963-113">Valitse lisätietojen pikaikkunassa **Lisätietoja**.</span><span class="sxs-lookup"><span data-stu-id="40963-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="40963-114">Lisätietoja poistetusta kohteesta (esimerkiksi aiherivi ja nimikkeen sijainti, kun se poistettiin) näkyvät **Vaikutuskohde-kentässä.**</span><span class="sxs-lookup"><span data-stu-id="40963-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="40963-115">**ClientInfoString-ominaisuus** näyttää, tapahtuiko poisto Outlookissa, Outlookin verkkoversiossa (aiemmin Outlook Web App) tai missä tahansa muussa laitteessa.</span><span class="sxs-lookup"><span data-stu-id="40963-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="40963-116">Lisätietoja on [ohjeaiheessa Postilaatikon sähköpostin edelleenlähetyksen määrittäminen](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="40963-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="40963-117">**Huomautus:** Poistettuja kohteita ei voi noutaa valvontalokitoiminnon avulla.</span><span class="sxs-lookup"><span data-stu-id="40963-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="40963-118">Lisätietoja poistettujen viestien noutamista Outlookin verkkoversiossa on [ohjeaiheessa Poistettujen kohteiden palauttaminen Outlook Web Appissa](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="40963-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
