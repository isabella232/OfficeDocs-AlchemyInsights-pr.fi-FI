---
title: Sovelluksen välityspalvelimen määritys
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7800"
ms.openlocfilehash: 835bfc59f77b31dc9a37c98db911505e2c7a758b37406dfc4da2d139afa61db5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951562"
---
# <a name="app-proxy-configuration"></a>Sovelluksen välityspalvelimen määritys

1. Lisätietoja sovelluksen välityspalvelimen sovelluksen määrittämisestä Azure AD:ssä paikallisiin sovelluksiin pilvessä on kohdassa Sovelluksen [välityspalvelimen sovelluksen määrittäminen.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)
2. Kertakirjautumisen avulla käyttäjät voivat käyttää sovellusta todentamatta useita kertoja. Sen avulla yksittäinen todennus voidaan suorittaa pilvipalvelussa, Azure Active Directory ja sen avulla palvelu tai Connector voi tekeytyä käyttäjäksi sovelluksen mahdolliset muut todennushaasteet. Lisätietoja on kohdassa [Kertakirjauksesi määrittäminen sovelluksen välityspalvelimen sovellukseen.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to)
3. Tämän [artikkelin avulla voit](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) tehdä vianmäärityksen yleisiin ongelmiin, joita ihmiset kohtaavat luodessaan uutta sovelluksen välityspalvelinsovellusta.
4. Jos sinulla on ongelmia sovelluksesi back-end-todennuksen määrittämisessä, sinun on ehkä [vianmääritystä Kerberosin](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) rajoitettujen delegointimääritysten vianmääritys sovelluksen välityspalvelinta varten tai määritettävä sovellus [PingAccessilla](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) ongelman ratkaisemiseksi.
