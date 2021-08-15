---
title: Eri porttien käyttö-ongelmien vianmääritys
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 07c108d5292965d20340da039b67744d93c0a4fc61edb8115796671f2f7f1552
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030899"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Eri porttien käyttö-ongelmien vianmääritys

Voit ratkaista eri porttien käyttöongelmat seuraavasti:

1. Pysäytä tai poista virtuaalikone (VM) portaalista, käynnistä virtuaalikone uudelleen ja testaa uudelleen. 
2. Tarkista virtuaalikoneen verkkoasetuksista, estääkö tietokoneesi liikenne verkon suojausryhmät. Verkon [Watcherin](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) IP-vuon tarkistustyökalun avulla voit myös tarkistaa, onko NSGs estävä liikenne, User-Defined Routes (UDRs) -reitittää liikenteen takaisin paikalliseen verkkoon (oletusreitti' 0.0.0.0/0) tai verkkolaite.
Jos ongelmia ilmenee edelleen yllä kuvattujen ohjeiden mukaisesti, anna virtuaalikoneen nimi ja TCP-portti, joita yrität lähettää sähköpostia lisädiagnosointiin.

**Suositellut asiakirjat**

[Rajoitukset ja suositukset lähtevän sähköpostin lähettämiseen portin 25 kautta](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)