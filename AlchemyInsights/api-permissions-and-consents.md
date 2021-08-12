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
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932094"
---
# <a name="api-permissions-and-consent"></a>Ohjelmointirajapinnan käyttöoikeudet ja suostumus

Sovellukset, jotka integroituvat Microsoftin käyttäjätietoympäristö seuraavat valtuutusmallia, jonka avulla käyttäjät ja järjestelmänvalvojat voivat hallita sitä, miten tietoja voidaan käyttää. Valtuutusmallin käyttöönotto on päivitetty Microsoftin käyttäjätietoympäristö päätepisteeseen. Se muuttaa tapaa, jolla sovelluksen on oltava vuorovaikutuksessa Microsoftin käyttäjätietoympäristö. [Käyttöoikeus- ja Microsoftin käyttäjätietoympäristö päätepiste](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) sisältää tämän valtuutusmallin peruskäsitteet, kuten laajuudet, käyttöoikeudet ja suostumuksen.

Azure Active Directory [(Azure AD) -suostumuskehys](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) helpottaa usean vuokraajan verkkosovellusten ja alkuperäisten asiakassovellusten kehittämistä. Nämä sovellukset sallivat kirjautumisen Azure AD -vuokraajan käyttäjätileillä, jotka ovat eri asia kuin sovelluksen rekisteröinti. Niiden on ehkä myös pääsy verkkorajapintojen, kuten Microsoft Graph -ohjelmointirajapinnan (Azure AD:n, Intunen ja Microsoft 365:n palvelujen) ja muiden Microsoft-palvelut:n ohjelmointirajapintojen, käyttöön omien verkkorajapintojen lisäksi.

