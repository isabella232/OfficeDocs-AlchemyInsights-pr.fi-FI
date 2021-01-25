---
title: Ohjelmointirajapinnan käyttöoikeudet ja suostumus
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974604"
---
# <a name="api-permissions-and-consent"></a>Ohjelmointirajapinnan käyttöoikeudet ja suostumus

Microsoftin tunnistetietoympäristöön integroivat sovellukset noudattavat valtuutusmallia, jonka avulla käyttäjät ja järjestelmänvalvojat voivat hallita, miten tietoja voidaan käyttää. Valtuutusmallin käyttöönotto on päivitetty Microsoftin tunnistetietoympäristön päätepisteeseen. Se muuttaa tapaa, jolla sovelluksen on oltava vuorovaikutuksessa Microsoftin käyttäjätietoympäristön kanssa. [Käyttöoikeudet ja suostumus Microsoftin](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) käyttäjätietoympäristön päätepisteissä kattavat tämän valtuutusmallin peruskäsitteet, mukaan lukien laajuus, käyttöoikeudet ja suostumus.

[Azure Active Directoryn (Azure AD) suostumuskehys](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) helpottaa usean vuokraajan verkko- ja alkuperäissovellusten kehittämistä. Nämä sovellukset sallivat kirjautumisen azure AD -vuokraajan käyttäjätileillä, jotka ovat eri asia kuin se, johon sovellus on rekisteröity. Heidän on ehkä myös päästä käyttämään verkkorajapintojen, kuten Microsoft Graphin ohjelmointirajapintaa (Azure AD:n, Intunen ja palveluiden käyttäminen Microsoft 365:ssä) ja muiden Microsoft-palveluiden ohjelmointirajapintojen lisäksi omia verkkorajapintojen lisäksi.

