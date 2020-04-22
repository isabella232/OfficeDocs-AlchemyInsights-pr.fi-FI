---
title: Valvontalokien sanomatapahtumien poistaminen
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
ms.openlocfilehash: 797a4b1146862faf91d2b9e8d74feade90f71650
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716493"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="b0d7d-102">Valvo poistettujen sähköpostiviestien lokit</span><span class="sxs-lookup"><span data-stu-id="b0d7d-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="b0d7d-103">Tammikuusta 2019 alkaen Microsoft ottaa postilaatikon valvontalokin käyttöön oletusarvoisesti.</span><span class="sxs-lookup"><span data-stu-id="b0d7d-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="b0d7d-104">Jos haluat tarkastella tietyn käyttäjän poistoviestitapahtumia, sinun on otettava poistotoiminnot valvonnan yhteydessä manuaalisesti käyttöön.</span><span class="sxs-lookup"><span data-stu-id="b0d7d-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="b0d7d-105">Jos postilaatikon valvontaloki on jo otettu käyttöön organisaatiossa tai tietylle käyttäjälle, noudata seuraavia ohjeita.</span><span class="sxs-lookup"><span data-stu-id="b0d7d-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="b0d7d-106">Kirjaudu Microsoft [365 Security & Compliance Centeriin](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="b0d7d-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="b0d7d-107">Valitse **Etsi ja tutki** ja valitse **Valvontalokin haku**.</span><span class="sxs-lookup"><span data-stu-id="b0d7d-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="b0d7d-108">Valitse päivämääräväli **Aloituspäivä-** ja **Päättymispäivä-kentissä.**</span><span class="sxs-lookup"><span data-stu-id="b0d7d-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="b0d7d-109">Määritä tutkittavan käyttäjän käyttäjänimi (käyttäjä, joka poisti kohteet).</span><span class="sxs-lookup"><span data-stu-id="b0d7d-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="b0d7d-110">Valitse **Aktiviteetit-kentässä** **Poistetut viestit Poistetut-kansiosta** ja **Siirretyt viestit Poistetut-kansioon**.</span><span class="sxs-lookup"><span data-stu-id="b0d7d-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="b0d7d-111">Valitse **Hae**.</span><span class="sxs-lookup"><span data-stu-id="b0d7d-111">Click **Search**.</span></span>

<span data-ttu-id="b0d7d-112">Valitse tuloksista valvontatietue.</span><span class="sxs-lookup"><span data-stu-id="b0d7d-112">In the results, select an audit record.</span></span> <span data-ttu-id="b0d7d-113">Valitse tiedot-pikaikkunassa **Lisätietoja**.</span><span class="sxs-lookup"><span data-stu-id="b0d7d-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="b0d7d-114">Lisätietoja poistetusta kohteesta (esimerkiksi aiherivi ja nimikkeen sijainti, kun se poistettiin) näkyy **Haavoittuvuuden kohteet** -kentässä.</span><span class="sxs-lookup"><span data-stu-id="b0d7d-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="b0d7d-115">**ClientInfoString-ominaisuus** näyttää, tapahtuiko poisto Outlookissa, Outlookin verkkoversiossa (aiemmin Outlook Web App) tai missä tahansa muussa laitteessa.</span><span class="sxs-lookup"><span data-stu-id="b0d7d-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="b0d7d-116">Lisätietoja on ohjeaiheessa [Postilaatikon sähköpostin edelleenlähetyksen määrittäminen](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="b0d7d-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="b0d7d-117">**Huomautus**: Et voi hakea poistettuja kohteita valvontalokiominaisuuden avulla.</span><span class="sxs-lookup"><span data-stu-id="b0d7d-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="b0d7d-118">Lisätietoja poistettujen viestien noutamiseen Outlookin verkkoversiossa on [ohjeaiheessa Poistettujen kohteiden palauttaminen Outlook Web Appissa](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="b0d7d-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
