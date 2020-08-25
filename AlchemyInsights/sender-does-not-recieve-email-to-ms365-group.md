---
title: Lähettäjä ei saa Microsoft 365-ryhmään lähetettyä sähkö postia
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/21/2020
ms.locfileid: "46871788"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Lähettäjä ei saa Microsoft 365-ryhmään lähetettyä sähkö postia

Sähkö posti viestin lähettäjä Microsoft 365-ryhmään ei oletusarvoisesti saa viestin kopiota Saapuneet-kansiostasi, vaikka Lähettäjä olisi ryhmän jäsen.

Käytä tätä EXO PowerShell-komentoa, jos haluat, että lähettäjä saa kopion jokaisesta lähettämänsä sähkö postista Microsoft 365-ryhmään:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Kaikkien posti laatikoiden asetusten ottaminen käyttöön samanaikaisesti:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Huomautus** Tämän asetuksen muutokset astuvat voimaan tunnin kuluttua.