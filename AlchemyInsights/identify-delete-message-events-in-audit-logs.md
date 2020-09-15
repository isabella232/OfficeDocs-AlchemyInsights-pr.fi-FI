---
title: Valvonta lokien Poista viesti tapahtumat-kohdan määrittäminen
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696510"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="137da-102">Poistettujen Sähkö posti viestien valvonta lokit</span><span class="sxs-lookup"><span data-stu-id="137da-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="137da-103">Tammi kuusta 2019 lähtien Microsoft on siirtymässä posti laatikon valvonta lokiin oletusarvoisesti.</span><span class="sxs-lookup"><span data-stu-id="137da-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="137da-104">Jos haluat tarkastella tietyn käyttäjän Poista viesti tapahtumia, sinun on otettava manuaalisesti käyttöön valvonnan poistamis toiminnot.</span><span class="sxs-lookup"><span data-stu-id="137da-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="137da-105">Jos posti laatikon valvonta loki on jo otettu käyttöön organisaatiossa tai tietyssä käyttäjälle, noudata seuraavia ohjeita.</span><span class="sxs-lookup"><span data-stu-id="137da-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="137da-106">Kirjaudu sisään [Microsoft 365-tieto turva & Compliance Centeriin](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="137da-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="137da-107">Valitse **haku ja tutkinta** ja valitse **valvonta lokien haku**.</span><span class="sxs-lookup"><span data-stu-id="137da-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="137da-108">Valitse päivämäärä väli **alkamis päivä** -ja **päättymis päivä** -kenttiin.</span><span class="sxs-lookup"><span data-stu-id="137da-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="137da-109">Määritä sen käyttäjän käyttäjä nimi, jonka haluat tutkia (kohteet poistaneen käyttäjän).</span><span class="sxs-lookup"><span data-stu-id="137da-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="137da-110">Valitse **aktiviteetit** -kentässä poistetut **viestit Poistetut-kansiosta** ja **siirretyt viestit Poistetut-kansioon**.</span><span class="sxs-lookup"><span data-stu-id="137da-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="137da-111">Valitse **Hae**.</span><span class="sxs-lookup"><span data-stu-id="137da-111">Click **Search**.</span></span>

<span data-ttu-id="137da-112">Valitse tulokset-kohdassa valvonta tietue.</span><span class="sxs-lookup"><span data-stu-id="137da-112">In the results, select an audit record.</span></span> <span data-ttu-id="137da-113">Valitse tiedot-valikosta **lisä tietoja**.</span><span class="sxs-lookup"><span data-stu-id="137da-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="137da-114">Lisä tietoja poistetusta kohteesta (esimerkiksi aihe-rivi ja kohteen sijainti, kun kohde on poistettu) näkyy **Affetecitems** -kentässä.</span><span class="sxs-lookup"><span data-stu-id="137da-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="137da-115">**Clialinfostring** -ominaisuus näkyy, jos poisto on tapahtunut Outlookissa, Outlookin verkko versiossa (aiemmin Outlook Web App) tai missä tahansa muussa laitteessa.</span><span class="sxs-lookup"><span data-stu-id="137da-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="137da-116">Lisä tietoja [on kohdassa sähkö postin lähettämisen määrittäminen Posti laatikolle](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="137da-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="137da-117">**Huomautus**: poistettuja kohteita ei voi noutaa valvonta loki-toiminnon avulla.</span><span class="sxs-lookup"><span data-stu-id="137da-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="137da-118">Lisä tietoja poistettujen viestien hakemisesta Outlookin verkko versiossa on Ohje aiheessa [poistettujen kohteiden palauttaminen Outlook Web Appissa](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="137da-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
