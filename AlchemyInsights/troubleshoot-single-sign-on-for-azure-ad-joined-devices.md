---
title: Kertakirjaaminen Azure AD:ssä liitettyjen laitteiden vianmääritys
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: 872333e13bb51b3a22431154627ad561f6db88c681c9eeee523fdd09e58c0371
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039243"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Kertakirjaaminen Azure AD:ssä liitettyjen laitteiden vianmääritys

Jos sinulla on paikallinen Active Directory (AD) -ympäristö ja haluat liittyä AD-toimialueeseen liitettyihin tietokoneisiin Azure AD:ssä, voit tehdä tämän Azure AD -yhdistelmäliitoksen avulla. [Toimintaohjeita: Yhdistelmäympäristön suunnitteleminen Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) käyttöönottoon liittyvien vaiheiden avulla voit toteuttaa Azure AD -yhdistelmäliitoksen ympäristössäsi.

Lisätietoja on kohdassa [Azure AD:lle liitettyjen](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)laitteiden määrittäminen paikallisille Single-Sign Windows Hello for Businessin avulla.

**PRT(Primary Refresh Token) -ongelmat**

Ensisijainen päivitystunnus (PRT) on Azure AD -todennuksen avainesiintyma Windows 10-, Windows Server 2016- ja sitä uudempien versioiden, iOS- ja Android-laitteiden kanssa. Se on JSON Web Token (JWT), joka on erityisesti myönnetty Microsoftin ensimmäisen osapuolen tunnuksen välittäjille, jotta kertakirjautuminen (SSO) voidaan ottaa käyttöön kyseisissä laitteissa käytetyissä sovelluksissa. Lisätietoja PRT-tunnuksen myöntäjästä, käytössä ja suojasta Windows 10-laitteissa on kohdassa Mikä on [ensisijainen päivitystunnus?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: YES ja AzureADPrt: YES**

Nämä kentät ilmaisevat, onko käyttäjä todennettu onnistuneesti Azure AD:ksi, kun hän kirjautuu laitteeseen. Jos arvot ovat **EI,** se voi johtua:

- Laitteeseen liitetyn TPM:n virheellinen tallennusavain rekisteröinnin yhteydessä (tarkista KeySignTest, kun käynnissä on laajennettu)
- Vaihtoehtoinen kirjautumistunnus
- HTTP-välityspalvelinta ei löydy

Lisätietoja laitteiden vianmäärityksestä dsregcmd-komennolla on kohdassa [SSO-tila.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
