---
title: Mikroviiveet tai rajoittaminen Exchange Online PowerShellissä
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: cb97aa790264c23aae15fed49c353c7fb0d6209d9492c6881f1b1091fe80d7b8
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/11/2021
ms.locfileid: "57868531"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikroviiveet tai rajoittaminen Exchange Online PowerShellissä

Kun suoritat Exchange Onlinessa komentosarjoja ja cmdlet-komentoja, saatat huomata viiveitä tai nähdä Mikroviive käytetty -varoituksen. Tässä on muutamia ehdotuksia, miten voit ratkaista ongelman:

- Suorita vianmääritys, niin voit rentoutua vuokraajan PowerShellin throtling-käytännöistä. Tämä ratkaisu ratkaisee ongelman useimmin.
- Jos ongelma ei ratkea vieläkään, [käytä Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)-moduulia, joka sisältää REST-ohjelmointirajapintaan perustuvat CMDlet-komennot, jotka toimivat huomattavasti tehokkaammin. Tämä voi olla hyvä ratkaisu monille usein käytettäville Get-CMDlet-komennoille.
- Jos sinun on käytettävä cmdlet-komentoja, joita ei sisällytetä v2-moduuliin, katso [PowerShellin cmdlet-komentojen](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)käyttö suurille käyttäjille Office 365:ssa, jossa käsitellään PowerShellin rajoitusrajoitusten käyttöä Exchange Online.
