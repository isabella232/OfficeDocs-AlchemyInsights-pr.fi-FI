---
title: Ulkoisten ryhmien poistaminen käytöstä
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/25/2019
ms.locfileid: "36739490"
---
# <a name="how-to-disable-external-groups"></a>Ulkoisten ryhmien poistaminen käytöstä

Yammerin ulkoinen viestintä käyttää Exchange-liikenne sääntöjä (ETF), joka on joukko ennakoivia ohjaus objekteja, jotka estävät yritys tietojen yhteistoiminnan. Jotta käyttäjät eivät voi luoda ulkoisia ryhmiä, sinun on määritettävä Exchange-siirto sääntö (ETR) ja määritettävä sitten Yammer käyttämään Exchange-siirto sääntöä ulkoisen Sanoman välityksen estämiseksi.
  
Kun olet luonut säännön Exchange Online-hallinta keskuksessa, määritä ETR-sovellus Yammerissa seuraavasti:
  
- Kirjaudu Yammeriin todennas-järjestelmänvalvojana ja **Yammerin hallinta keskuksessa**kohtaan C **Content ja Security \> Security Settings.**

- Valitse **ulkoiset viestit**-kohdassa **Pakota Exchange Online Exchange-siirto sääntösi (ETR) Yammerissa.**

- Valitse **Tallenna**.

Lisä tietoja on kohdassa [ulkoisten viestien poistaminen käytöstä Yammer-verkossa](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  