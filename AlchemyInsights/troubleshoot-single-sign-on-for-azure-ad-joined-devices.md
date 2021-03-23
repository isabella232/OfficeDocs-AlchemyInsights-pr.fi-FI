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
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035468"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Kertakirjaaminen Azure AD:ssä liitettyjen laitteiden vianmääritys

Jos sinulla on paikallinen Active Directory (AD) -ympäristö ja haluat liittyä AD-toimialueeseen liitettyihin tietokoneisiin Azure AD:ssä, voit tehdä tämän tekemällä Azure AD -yhdistelmäliitoksen. [Toimintaohjeita: Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) -yhdistelmäympäristön käyttöönottoon liittyvien vaiheiden avulla voit toteuttaa Azure AD -yhdistelmäliitoksen ympäristössäsi.

Lisätietoja on kohdassa Azure AD:n liitettyjen laitteiden määrittäminen [paikallisille Single-Sign Windows Hello for Businessin käyttöön.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)

**PRT (Primary Refresh Token) -ongelmat**

Ensisijainen päivitystunnus (PRT) on Azure AD -todennuksen tärkeä artefakti Windows 10-, Windows Server 2016- ja sitä uudemmassa versiossa, iOS- ja Android-laitteissa. Se on JSON Web Token (JWT), joka on erityisesti myönnetty Microsoftin ensimmäisen osapuolen tunnuksen välittäjänä, jotta kertakirjautuminen (SSO) voidaan ottaa käyttöön kaikissa näissä laitteissa käytetyissä sovelluksissa. Lisätietoja PRT:n myöntäjästä, käytössä ja suojasta Windows 10 -laitteissa on ohjeaiheessa Mikä on [ensisijainen päivitystunnus?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: KYLLÄ ja AzureADPrt: KYLLÄ**

Nämä kentät ilmaisevat, onko käyttäjä onnistunut todentamaan Azure AD:n, kun kirjaudut sisään laitteeseen. Jos arvot ovat **EI,** se voi johtua:

- Laitteeseen liitetyn TPM:n virheellinen tallennustilaavain rekisteröinnin yhteydessä (tarkista KeySignTest, kun käynnissä on laajennettuna)
- Vaihtoehtoinen kirjautumistunnus
- HTTP-välityspalvelinta ei löydy

Lisätietoja laitteiden vianmäärityksestä dsregcmd-komennolla on kohdassa [SSO-tila.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
