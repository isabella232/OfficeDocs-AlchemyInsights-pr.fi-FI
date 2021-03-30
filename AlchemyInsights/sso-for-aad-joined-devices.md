---
title: Single-Sign Azure Active Directoryyn liitettyjen laitteiden käyttöön
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404592"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Kertakirjaminen Azure Active Directoryyn yhdistetyissä laitteissa

Jos käytössäsi on paikallinen Active Directory (AD) -ympäristö ja haluat liittyä AD-toimialueeseen liitettyihin tietokoneisiin Azure AD:ssä, voit tehdä tämän tekemällä Azure AD -yhdistelmäliitoksen. [Toimintaohjeita: Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) -yhdistelmäympäristön käyttöönottoon liittyvien vaiheiden avulla voit toteuttaa Azure AD -yhdistelmäliitoksen ympäristössäsi.

[Azure AD:ssä liitettyjen laitteiden määrittäminen paikallisille Single-Sign Käytössä Windows Hello for Businessin avulla](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**PRT (Primary Refresh Token) -ongelmat** Ensisijainen päivitystunnus (PRT) on Azure AD -todennuksen tärkeä artefakti Windows 10-, Windows Server 2016- ja sitä uudemmassa versiossa, iOS- ja Android-laitteissa. Se on JSON Web Token (JWT), joka on erityisesti myönnetty Microsoftin ensimmäisen osapuolen tunnuksen välittäjänä, jotta kertakirjautuminen (SSO) voidaan ottaa käyttöön kaikissa näissä laitteissa käytetyissä sovelluksissa. Mikä on [ensisijainen päivitystunnus?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)-kohdassa annetaan tietoja siitä, miten PRT myönnetään, käytetään ja suojataan Windows 10 -laitteissa.

**WamDefaultSet: KYLLÄ ja AzureADPrt: KYLLÄ** Nämä kentät ilmaisevat, onko käyttäjä onnistunut todentamaan Azure AD:n, kun hän kirjautuu laitteeseen. Jos arvot ovat **EI,** se voi olla erääntymispäivä:

- Laitteeseen liitetyn TPM:n virheellinen tallennustilaavain rekisteröinnin yhteydessä (tarkista KeySignTest, kun käynnissä on järjestelmänvalvojana).
- Vaihtoehtoinen kirjautumistunnus
- HTTP-välityspalvelinta ei löydy

Laitteiden vianmääritys dsregcmd-komennolla – [SSO-tila](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
