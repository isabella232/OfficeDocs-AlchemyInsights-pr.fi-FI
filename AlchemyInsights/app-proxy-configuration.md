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
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885131"
---
# <a name="app-proxy-configuration"></a>Sovelluksen välityspalvelimen määritys

1. Lisätietoja sovellusten välityspalvelimen sovelluksen määrittämisestä Azure AD:ssä, jotta paikallissovellukset voidaan näyttää pilvipalvelussa, on kohdassa Sovelluksen [välityspalvelinsovelluksen määrittäminen.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)
2. Kertakirjautumisen avulla käyttäjät voivat käyttää sovellusta todentamatta useita kertoja. Sen avulla yksittäinen todennus voidaan suorittaa pilvessä Azure Active Directorya vastaan ja sen avulla palvelu tai yhdistin voi tekeytyä käyttäjän sovelluksesta syntyviin muihin todennushaasteisiin. Lisätietoja on kohdassa [Kertakirjauksesi määrittäminen sovelluksen välityspalvelinsovellukseen.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to)
3. Tämän [artikkelin avulla voit](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) tehdä vianmäärityksen yleisiin ongelmiin, joita ihmiset kohtaavat luotaessa uutta sovelluksen välityspalvelinsovellusta.
4. Jos sinulla on ongelmia sovelluksesi taustatodentamisen määrittämisessä, sinun on ehkä [vianmääritystä Kerberosin](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) rajoitettuja delegointimäärityksiä sovelluksen välityspalvelinta varten tai seurattava ohjeita sovelluksen määrittämiseen [PingAccessilla](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) ongelman ratkaisemiseksi.
