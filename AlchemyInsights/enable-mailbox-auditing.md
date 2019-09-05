---
title: Ota käyttöön posti laatikon valvonta
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736250"
---
# <a name="enable-mailbox-auditing"></a>Ota käyttöön posti laatikon valvonta

Jos haluat ottaa posti laatikon valvonnan käyttöön joko yksittäisessä tai koko organisaatiossa, seuraavat cmdlet-komennot on suoritettava Etävirralla:
  
 **Yksittäinen käyttäjä**
  
Set-posti laatikko-identiteetti "Jane Dow"-AuditEnabled $true
  
 **Organisaatio**
  
Get-posti laatikko-ResultSize Unlimited-suodatin {Vastaanottaenttypedetails-EQ "Userposti laatikko"} | Aseta-posti laatikko-AuditEnabled $true
  
[Opi lisää](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

