---
title: Ulkoisten ryhmien poistaminen käytöstä
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720765"
---
# <a name="how-to-disable-external-groups"></a>Ulkoisten ryhmien poistaminen käytöstä

Yammerin ulkoiset viestit käyttävät Exchange Transport Rules (ETRs) -sääntöjä, jotka ovat joukko ennakoivia ohjausobjekteja, jotka estävät yrityksen tietojen jakamisen. Jotta voit estää käyttäjiä luomasta ulkoisia ryhmiä, sinun on määritettävä Exchange-siirtosääntö (ETR) ja määritettävä Yammer estämään ulkoiset viestit Exchange Transport -säännön avulla.
  
Kun olet luonut säännön Exchange Online -hallintakeskuksessa, määritä ETR-arvo Yammerissa seuraavasti:
  
- Kirjaudu Yammeriin vahvistetuna järjestelmänvalvojana ja siirry **Yammer-hallintakeskukseen**kohtaan C **Content and Security Settings (C-sisältö- ja suojausasetukset). \> **

- Valitse **Ulkoiset viestit -kohdassa** **Pakota Exchange Online Exchange -siirtosäännöt (Etr) Yammerissa.**

- Valitse **Tallenna**.

Lisätietoja on [ohjeaiheessa Ulkoisten viestien poistaminen käytöstä Yammer-verkossa](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  