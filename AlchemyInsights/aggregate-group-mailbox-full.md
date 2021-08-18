---
title: AggregateGroupMailbox, joka on saanut täydellisen NDR-viestin Microsoft 365 ryhmälle
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
ms.openlocfilehash: ace8e256e3771f82512abcb9e20b832381eedf80
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315907"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox, joka on saanut täydellisen NDR-viestin Microsoft 365 ryhmälle

Seuraavan EXO Shell -komennon avulla voit luoda Exchange, joka hiljaisesti pudottaa koosteryhmäpostilaatikkoon lähetetyt sähköpostiviestit:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

**Huomautus:** Korvaa **-SentTo-viestin SMTP-osoite** vuokraajan koosteryhmän postilaatikon SMTP-osoitteella. Voit saada koosteryhmän postilaatikon SMTP-osoitteen NDR-palvelimesta.



