---
title: 1065 EOP:n lähtevän liikenteen IP-osoitealueen poistoMC146155
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
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031259"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>EOP:n lähtevien IP-osoitevälien poisto

Olemme havainneet mahdollisen ongelman organisaatiossasi, joka (jos sitä ei ole korjattu 26. lokakuuta 2018 mennessä) saattaa katkaista postinkulkua paikallisiin tai ulkoisiin kohteisiin. Kuten aiemmin on ilmoitettu, IP-osoitealueen hallinnan yksinkertaistamiseksi yhdistämme Exchange Online Protection (EOP) -IP-osoite alueet, joita käytetään sähköpostin lähettämiseen ja vastaanottamiseen Microsoft 365. Analyysimme osoittaa, että yksi tai useampi sähköpostin lähteistä tai kohteista, jotka olet määrittänyt postinkulkuyhdistimiin, ei hyväksy yhteyksiä tässä näytettäviltä [IP-osoitealueista.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Varmista ennen 26. lokakuuta, että nämä lähteet ja kohteet hyväksyvät yhteydet kaikkiin julkaistuihin [EOP:n IP-osoitteisiin ja niistä.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Lisätietoja muutoksesta on kohdassa Viestikeskuksen viestit [MC146155,](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155) [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)tai [MC149274.](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)

**Huomautus:** Jos olet aiemmin käyttänyt IP- tai URL-osoitteiden julkaisemista HTML-, XML- ja RSS-protokollan kautta päätepistepäivityksiä varten, sinun on myös siirrettävä uusiin verkkopalveluihin tämäntyyppisten päivitysten automatisointiin. Lisätietoja on luokkien Microsoft 365 ja [IP Microsoft 365 osoite- ja URL-verkkopalvelun ohjeissa.](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)
