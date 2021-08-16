---
title: Ota selvää, kuka on määrittänyt edelleenlähetystä postilaatikossa ja miten
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6243e787bb6b51f26cf22782d9ec80f946430b864f53de7ea626b7166a674d2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988196"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Ota selvää, kuka on määrittänyt edelleenlähetystä postilaatikossa ja miten

Jos postilaatikossa on määritetty ulkoinen edelleenlähetys, toiminta valvotaan osana Set-Mailbox cmdlet-komentoa. Voit etsiä toiminnon valvontalokista näin:

1. Siirry Office 365 [tietoturva- & yhteensopivuuskeskukseen.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Valitse **Haun** >  **valvontalokihaku**.
    > [!NOTE]
    > Jos huomaat, että valvonta on syytä ottaa käyttöön, ota se käyttöön nyt. Jos tämä toiminto ei ole käytössä, hakutulokset eivät voi hakea tietoja aiemmista päivämääristä.
1. Varmista, että **Toiminnot-kentän** arvoksi **on määritetty Näytä kaikkien toimintojen tulokset** (oletus). Määritä päivämääräalue. Käyttäjänimeä ei tarvitse määrittää.
1. Valitse **Hae**. Toiminnot näkyvät **Tulokset-kohdassa.**
1. Valitse **Suodata** tulokset ja kirjoita sitten **Määritä postilaatikkoToiminta-suodatinkenttään.**  Tämä palauttaa kaikki **Set-Mailbox-toiminnot.**
1. Voit tarkastella tietoja valitsemalla aktiviteetin ja valitsemalla sitten **Lisätietoja**. **Parametrit-kohdassa** näet postilaatikossa olevan edelleenlähetyssähköpostiosoitteen. UserID **edustaa** käyttäjää, joka on määrittänyt postilaatikossa ulkoisen edelleenlähetyspalvelun.
Lisätietoja on ohjeaiheessa [Valvontalokin Office 365 ja yleisimmät skenaariot.](https://go.microsoft.com/fwlink/?linkid=2103944)