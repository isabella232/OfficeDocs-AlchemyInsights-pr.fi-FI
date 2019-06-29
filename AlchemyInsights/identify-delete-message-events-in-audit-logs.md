---
title: Seurantalokien poistaminen viestin tapahtumien selvittäminen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 89877331d328d798177fab3150d5219c5b484a70
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383130"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="4c02f-102">Postitettujen viestien valvontalokissa.</span><span class="sxs-lookup"><span data-stu-id="4c02f-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="4c02f-103">Tammikuuta 2019 alkaen Microsoft on ottaminen käyttöön postilaatikon valvonta on oletusarvon mukaan kirjaaminen.</span><span class="sxs-lookup"><span data-stu-id="4c02f-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="4c02f-104">Muussa tapauksessa poista viesti tapahtumia tietyn käyttäjän tarkastelemaan täytyy ottaa käyttöön manuaalisesti Poista toimintojen valvonta</span><span class="sxs-lookup"><span data-stu-id="4c02f-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="4c02f-105">Jos postilaatikon valvonnan kirjaaminen on jo käytössä organisaation tai tietyn käyttäjän, alla olevien ohjeiden mukaisesti.</span><span class="sxs-lookup"><span data-stu-id="4c02f-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="4c02f-106">Kirjautua [Office 365-suojauksen & Compliance Centeriin](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="4c02f-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="4c02f-107">**Etsi ja tutkimus** ja valitse **Valvo lokista etsintää**.</span><span class="sxs-lookup"><span data-stu-id="4c02f-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="4c02f-108">Valitse **aloituspäivä** - ja **päättymispäivä** -kenttiin päivämääräalue.</span><span class="sxs-lookup"><span data-stu-id="4c02f-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="4c02f-109">Määritä käyttäjänimi käyttäjä, jonka haluat tutkia (käyttäjä joka poistaa nimikkeitä).</span><span class="sxs-lookup"><span data-stu-id="4c02f-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="4c02f-110">Valitse **aktiviteetit** -kentässä **Poistetut viestit Poistetut-kansiosta** ja **Moved viestit Poistetut-kansioon**.</span><span class="sxs-lookup"><span data-stu-id="4c02f-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="4c02f-111">Valitse **Etsi**.</span><span class="sxs-lookup"><span data-stu-id="4c02f-111">Click **Search**.</span></span>

<span data-ttu-id="4c02f-112">Valitse tulosten koskeva seurantatietue.</span><span class="sxs-lookup"><span data-stu-id="4c02f-112">In the results, select an audit record.</span></span> <span data-ttu-id="4c02f-113">Valitse tiedot-valikon avauspainike **Lisätietoja**.</span><span class="sxs-lookup"><span data-stu-id="4c02f-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="4c02f-114">**AffectedItems** -kentässä näkyy lisätietoja poistetun kohteen (esimerkiksi aihe ja sijainti kohde, kun se on poistettu).</span><span class="sxs-lookup"><span data-stu-id="4c02f-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="4c02f-115">**ClientInfoString** -ominaisuus näyttää, jos Outlookissa, Outlook web (tunnettiin aiemmin nimellä Outlook Web App), tai muussa laitteessa tapahtunut poisto.</span><span class="sxs-lookup"><span data-stu-id="4c02f-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="4c02f-116">Lisätietoja [määrittäminen, joka määrittää sähköpostiviestin välittäminen postilaatikkoon](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="4c02f-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="4c02f-117">**Huomautus**: audit log-toiminnolla poistettuja kohteita ei voi noutaa.</span><span class="sxs-lookup"><span data-stu-id="4c02f-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="4c02f-118">Noutamaan poistetut viestit Outlook Web-kohdassa [Palauta poistetut viestit Outlook Web Appissa](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="4c02f-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
