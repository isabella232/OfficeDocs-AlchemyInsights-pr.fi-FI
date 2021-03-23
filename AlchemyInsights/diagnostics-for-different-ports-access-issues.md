---
title: Eri porttien käyttöongelmien vianmääritys
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
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035261"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Eri porttien käyttöongelmien vianmääritys

Voit ratkaista eri porttien käyttöongelmat seuraavasti:

1. Pysäytä tai poista virtuaalikone (VM) portaalista, käynnistä virtuaalikone uudelleen ja testaa uudelleen. 
2. Tarkista virtuaalikoneen verkkoasetukset ja tarkista, estääkö verkon käyttöoikeusryhmät (NSGs) liikenteen. Verkon [Watcherin IP-liikenteen](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) tarkistustyökalun avulla voit myös tarkistaa, estääkö NSGs liikenteen, User-Defined Routes (UDRs) -reitit ( UdRs) uudelleenreitittää liikenteen takaisin paikalliseen paikalliseen (Oletusreititys 0.0.0.0/0) tai verkkolaite.
Jos sinulla on edelleen ongelmia edellä kuvattujen vaiheiden koettamisen jälkeen, anna virtuaalikoneen nimi ja TCP-portti, jossa yrität lähettää sähköpostia lisädiagnosointiin.

**Suositellut asiakirjat**

[Portin 25 kautta lähtevän sähköpostin lähettämisen rajoitukset ja suositukset](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)