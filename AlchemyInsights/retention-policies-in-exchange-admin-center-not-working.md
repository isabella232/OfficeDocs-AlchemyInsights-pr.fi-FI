---
title: Exchange-hallintakeskuksen säilytyskäytännöt eivät toimi
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 6652ad5fc1691e1d5a4293d81f3a649f23ec38f18c8ed9fe06665628a901d13e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074929"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Exchange säilytyskäytännöt

Jos haluat, että suoritamme automaattiset tarkistukset alla mainittujen asetusten varalta, valitse Sivun yläreunassa Takaisin-painike < ja kirjoita sitten sen käyttäjän sähköpostiosoite, jolla on ongelmia säilytyskäytäntöjen kanssa.

Jos sinulla on ongelmia Exchange-hallintakeskuksen säilytyskäytäntöjen kanssa, jotka eivät koske postilaatikoita tai kohteita, jotka eivät siirry arkistopostilaatikkoon, tarkista seuraavat asiat:

**Perimmäinen syy:**

- **Kansion hallinta -avustaja** ei ole käsitellyt käyttäjän postilaatikkoa. Hallitun kansion avustaja yrittää käsitellä pilvipohjaisen organisaation jokaista postilaatikkoa seitsemän päivän välein.

  **Ratkaisu:** Suorita Kansion hallinta -avustaja.

- **RetentionHold** on **otettu** käyttöön postilaatikossa. Jos postilaatikko on sijoitettu RetentionHold-kohteelle, postilaatikon säilytyskäytäntöä ei käsitellä kyseisenä aikana.

  **Ratkaisu:** Tarkista säilytysten pitoasetuksen tila ja päivitä se tarvittaessa. Lisätietoja on kohdassa [Postilaatikon säilytys .](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
 
**Huomautus:** Jos postilaatikon koko on alle 10 Mt, Kansion hallinta -avustaja ei käsittele postilaatikkoa automaattisesti.
 
Lisätietoja Exchange säilytyskäytännöistä:

- [Säilytystunnisteet ja säilytyskäytännöt](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Säilytyskäytännön käyttäminen postilaatikoissa tai](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) [Säilytystunnisteiden lisääminen tai poistaminen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Postilaatikon pitotyypin tunnistaminen](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
