---
title: Oletusmerkintä Outlook asetusta ei käytetä
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/17/2021
ms.locfileid: "58454756"
---
# <a name="default-outlook-label-setting-not-applied"></a>Oletusmerkintä Outlook asetusta ei käytetä

Jos Outlook-oletusasetukset eivät ole käytössä oikein ja jos käytössä on eri selite tai selite ei ole käytössä, ongelma voi olla tiedossa (MC277818) ja ratkaise ongelma jommankumman seuraavista 2 vaihtoehdosta:

**Vaihtoehto 1:**

1. Siirry Microsoft 365 -> **ratkaisuihin.**  >  
1. Valitse **Osoitetarrakäytännöt** ja valitse muokattava osoitetarrakäytäntö (**OutlookDefaultlabel** -asetusta ei ole määritetty oikein kyse ässä tarrakäytäntöön. Tarkastele **tätä asetusta suorita Get-labelpolicy)** ja valitse sitten Muokkaa **käytäntöä**.
1. Valitse **Seuraava,** kunnes näet Käytä tätä oletusmerkintää sähköposteihin  -asetuksen **,** joka on käytettävissä, jos valitset Käytäntöasetukset-valintaikkunassa Edellytä, että käyttäjät soveltavat selitetä perimerkkisähköposteihin ja **asiakirjoihin.**
1. Valitse Käytä **oletusotsikoita asiakirjoihin** -valintaikkunassa  Ei mitään avattavasta luettelosta.
1. Tallenna **osoitetarra-asetukset** valitsemalla Seuraava ja Lähetä. 

**Vaihtoehto 2:**

Käytä [Tietoturva- ja yhteensopivuuskeskuksessa Powershellin](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)Set-LabelPolicy-komentoa **muuttaaksesi OutlookDefaultlabelin** **arvoksi** Ei mitään kohteessa {OutlookDefaultLabel="None"}.

Suorita: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

Lisätietoja oletusotsikoista on Outlook kohdassa Eri [oletusotsikoiden Outlook.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook)