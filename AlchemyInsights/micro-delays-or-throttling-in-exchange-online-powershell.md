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
ms.openlocfilehash: 6753dcb375ea5e19b01c4350b61aa8904aa102112df175a3f70281d18a634dbf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098563"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikroviiveet tai rajoittaminen Exchange Online PowerShellissä

Kun suoritat Exchange Onlinessa komentosarjoja ja cmdlet-komentoja, saatat huomata viiveitä tai nähdä Mikroviive käytetty -varoituksen. Tässä on muutamia ehdotuksia, miten voit ratkaista ongelman:

- Suorita vianmääritys, niin voit rentoutua vuokraajan PowerShellin throtling-käytännöistä. Tämä ratkaisu ratkaisee ongelman useimmin.
- Jos ongelma ei ratkea vieläkään, [käytä Exchange Online v2 PowerShell](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)-moduulia, joka sisältää REST-ohjelmointirajapintaan perustuvat CMDlet-komennot ja jotka toimivat huomattavasti tehokkaammin. Tämä voi olla hyvä ratkaisu monille usein käytettäville Get-CMDlet-komennoille.
- Jos sinun on käytettävä CMDlet-komentoja, joita ei sisällytetä v2-moduuliin, katso [PowerShellin cmdlet-komentojen](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)käyttö suurille käyttäjille Office 365:ssä, jossa käsitellään PowerShellin rajoitusrajoitusten Exchange Online.
