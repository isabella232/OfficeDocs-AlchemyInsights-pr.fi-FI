---
title: Single-Sign käyttöön Azure Active Directory laitteissa
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
ms.openlocfilehash: 365225926296677feb7853481651a634792fd8bfa9abd9dc9359ffaae50b60eb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050007"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Kertakirjaminen Azure Active Directory laitteiden kanssa

Jos sinulla on paikallinen Active Directory (AD) -ympäristö ja haluat liittyä AD-toimialueeseen liitettyihin tietokoneisiin Azure AD:ssä, voit tehdä tämän Azure AD -yhdistelmäliitoksen avulla. [Toimintaohjeita: Yhdistelmäympäristön suunnitteleminen Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) käyttöönottoon liittyvien vaiheiden avulla voit toteuttaa Azure AD -yhdistelmäliitoksen ympäristössäsi.

[Azure AD:lle liitettyjen laitteiden määrittäminen paikallisille Single-Sign käytössä Windows Hello for Businessin avulla](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**PRT(Primary Refresh Token) -ongelmat** Ensisijainen päivitystunnus (PRT) on Azure AD -todennuksen avainesiintyma Windows 10-, Windows Server 2016- ja sitä uudempien versioiden, iOS- ja Android-laitteiden kanssa. Se on JSON Web Token (JWT), joka on erityisesti myönnetty Microsoftin ensimmäisen osapuolen tunnuksen välittäjille, jotta kertakirjautuminen (SSO) voidaan ottaa käyttöön kyseisissä laitteissa käytetyissä sovelluksissa. [Mitä on ensisijainen päivitystunnus?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)-kohdassa annetaan tietoja SIITÄ, miten PRT-tunnus myönnetään, käytetään ja suojataan Windows 10 laitteissa.

**WamDefaultSet: YES ja AzureADPrt: YES** Nämä kentät ilmaisevat, onko käyttäjä todennettu onnistuneesti Azure AD:ksi, kun hän kirjautuu laitteeseen. Jos arvot ovat **EI,** se saattaa erääntyä:

- Virheellinen tallennustilaavain laitteeseen liitetyssä TPM:ssä rekisteröinnin yhteydessä (tarkista KeySignTest, kun käynnissä on laajennettuna).
- Vaihtoehtoinen kirjautumistunnus
- HTTP-välityspalvelinta ei löydy

Laitteiden vianmääritys dsregcmd-komennolla – [SSO-tila](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
