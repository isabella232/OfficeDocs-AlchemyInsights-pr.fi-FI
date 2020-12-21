---
title: Aggrecategroupmailbox vastaanotettu Microsoft 365-ryhmälle lähetetyt sähkö postit.
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: 9de09ab4cbd2f09648305b11da6273ed990907cf
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/18/2020
ms.locfileid: "49721921"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>Aggrecategroupmailbox vastaanotettu Microsoft 365-ryhmälle lähetetyt sähkö postit.

Käytä seuraavaa EXO Shell-komentoa, kun haluat luoda Exchange-siirto säännön, jonka avulla voit poistaa sähkö postit, jotka on lähetetty kooste ryhmän posti laatikkoon

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> Vaihda SMTP-osoite in **-Sento-** kohdassa, jossa on palveltavan kooste ryhmän posti laatikon SMTP-osoite. Voit hankkia kooste ryhmän posti laatikon SMTP-osoitteen vastaanotetun NDR-ilmoituksen perusteella.



