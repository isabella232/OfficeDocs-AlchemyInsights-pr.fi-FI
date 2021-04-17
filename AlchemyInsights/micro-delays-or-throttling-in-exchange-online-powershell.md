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
ms.openlocfilehash: 680df9e6e2404ff6b60b17d6ac88e202e9a7bb25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830030"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikroviiveet tai rajoittaminen Exchange Online PowerShellissä

Kun suoritat Exchange Onlinessa komentosarjoja ja cmdlet-komentoja, saatat huomata viiveitä tai nähdä Mikroviive käytetty -varoituksen. Seuraavassa on kaksi tähän liittyvää ehdotusta:

- Sinun kannattaa ehkä kokeilla [Exchange Online v2 PowerShell -moduulia](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), joka sisältää REST-ohjelmointirajapintaan perustuvia, paljon paremmin toimivia CMDlet-komentoja. Tämä voi olla hyvä ratkaisu monille usein käytettäville Get-CMDlet-komennoille.
- Jos haluat käyttää CMDlet-komentoja, joita v2-moduuli ei kata vielä, tutustu artikkeliin [PowerShell cmdlet -komentojen suorittaminen suurille käyttäjämäärille Office 365:ssä](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), jossa kerrotaan, miten odotetut PowerShellin rajoitukset voidaan kiertää Exchange Onlinessa.
