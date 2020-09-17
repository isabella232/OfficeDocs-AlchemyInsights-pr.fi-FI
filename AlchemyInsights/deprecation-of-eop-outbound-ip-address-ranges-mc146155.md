---
title: 1065 poistumisesta, lähtevä IP-osoite rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806792"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Poistumisesta-lähtevien IP-osoitteiden alueet

Olemme havainneet, että organisaatioosi liittyy mahdollisesti ongelma, joka (jos sitä ei ole korjattu 26. loka kuuta, 2018) saattaa rikkoa sähkö postin kulkua paikallisiin tai ulkoisiin kohteisiin. Kuten aiemmin ilmoitettiin, voit yksinkertaistaa IP-osoite alueen hallintaa yhdistämällä Exchange Online Protection (ESIP)-IP-osoite alueet, joita käytetään sähkö postin lähettämiseen ja vastaanottoon Microsoft 365: n ulkopuolella. Analyysimme osoittaa, että vähintään yksi sähkö postin kulku yhdistimiin määritetyistä ulkoisista Sähkö posti lähteistä tai kohteista ei hyväksy yhteyksiä [tässä](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)näytetyn IP-osoite alueen kautta.

Toimi ennen 26 päivää loka kuuta varmistaaksesi, että nämä lähteet ja kohteet hyväksyvät yhteydet kaikkiin julkaistujen Sähkö posti [OSOITTEIDEN IP-osoitteisiin](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Lisä tietoja tästä muutoksesta on kohdassa viesti keskuksen viestit [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)tai [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Huomautus**: Jos olet käyttänyt IP-tai URL-julkaisua aiemmin HTML:n, XML:n ja RSS-syötteiden kautta pääte piste päivityksissä, sinun on myös siirryttävä uusiin verkko palveluihin tämäntyyppisten päivitysten automatisoimiseksi. Lisä tietoja on kohdassa [microsoft 365-pääte piste luokat ja microsoft 365 IP-osoite ja URL-verkko palvelu](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
