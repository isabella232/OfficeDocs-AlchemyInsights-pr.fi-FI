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
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="7f9aa-102">Eri porttien käyttöongelmien vianmääritys</span><span class="sxs-lookup"><span data-stu-id="7f9aa-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="7f9aa-103">Voit ratkaista eri porttien käyttöongelmat seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="7f9aa-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="7f9aa-104">Pysäytä tai poista virtuaalikone (VM) portaalista, käynnistä virtuaalikone uudelleen ja testaa uudelleen.</span><span class="sxs-lookup"><span data-stu-id="7f9aa-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="7f9aa-105">Tarkista virtuaalikoneen verkkoasetukset ja tarkista, estääkö verkon käyttöoikeusryhmät (NSGs) liikenteen.</span><span class="sxs-lookup"><span data-stu-id="7f9aa-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="7f9aa-106">Verkon [Watcherin IP-liikenteen](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) tarkistustyökalun avulla voit myös tarkistaa, estääkö NSGs liikenteen, User-Defined Routes (UDRs) -reitit ( UdRs) uudelleenreitittää liikenteen takaisin paikalliseen paikalliseen (Oletusreititys 0.0.0.0/0) tai verkkolaite.</span><span class="sxs-lookup"><span data-stu-id="7f9aa-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="7f9aa-107">Jos sinulla on edelleen ongelmia edellä kuvattujen vaiheiden koettamisen jälkeen, anna virtuaalikoneen nimi ja TCP-portti, jossa yrität lähettää sähköpostia lisädiagnosointiin.</span><span class="sxs-lookup"><span data-stu-id="7f9aa-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="7f9aa-108">**Suositellut asiakirjat**</span><span class="sxs-lookup"><span data-stu-id="7f9aa-108">**Recommended Documents**</span></span>

[<span data-ttu-id="7f9aa-109">Portin 25 kautta lähtevän sähköpostin lähettämisen rajoitukset ja suositukset</span><span class="sxs-lookup"><span data-stu-id="7f9aa-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)