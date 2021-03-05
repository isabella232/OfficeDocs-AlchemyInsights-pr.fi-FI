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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481574"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Ota selvää, kuka on määrittänyt edelleenlähetystä postilaatikossa ja miten

Jos postilaatikossa on määritetty ulkoinen edelleenlähetys, toiminta valvotaan osana Set-Mailbox cmdlet-komentoa. Näin löydät toiminnon valvontalokista:

1. Siirry [Office 365:n tietoturva- & yhteensopivuuskeskukseen.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Valitse **Haun** >  **valvontalokihaku.**
    > [!NOTE]
    > Jos näet ilmoituksen, että valvonta on syytä ottaa käyttöön, ota se käyttöön nyt. Jos tätä ominaisuutta ei ole otettu käyttöön, hakutulokset eivät voi hakea tietoja aiemmista päivämääristä.
1. Varmista, että **Toiminnot-kentän** **arvoksi on määritetty Näytä kaikkien toimintojen** tulokset (oletus). Määritä päivämääräalue. Käyttäjänimeä ei tarvitse määrittää.
1. Valitse **Hae.** Toiminnot näkyvät **Tulokset-kohdassa.**
1. Valitse **Suodata** tulokset ja kirjoita sitten **Aseta-postilaatikko** **Toimintasuodatin-kenttään.** Tämä palauttaa kaikki **Set-Mailbox-toiminnot.**
1. Voit tarkastella tietoja valitsemalla aktiviteetin ja valitsemalla sitten **Lisätietoja.** **Parametrit-kohdassa** näet postilaatikossa olevan edelleenlähetyssähköpostiosoitteen. Käyttäjätunnus **edustaa** käyttäjää, joka on määrittänyt postilaatikossa ulkoisen edelleenlähetyspalvelun.
Lisätietoja on ohjeaiheessa Office [365:n valvontalokista etsiminen yleisimpiä skenaarioita varten.](https://go.microsoft.com/fwlink/?linkid=2103944)