---
title: 1065 EOP:n lähtevien IP-osoitealueiden POISTOMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704594"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>EOP:n lähtevien IP-osoitealueiden poisto

Olemme havainneet organisaatiossasi mahdollisen ongelman, joka saattaa (jos sitä ei korjata 26.10.2018 mennessä) saattaa katkaista postivirran paikallisiin tai ulkoisiin kohteisiin. Kuten aiemmin ilmoitettiin, ip-osoitealueen hallinnan yksinkertaistamiseksi konsolidoimme Exchange Online Protectionin (EOP) IP-osoitealueet, joita käytetään sähköpostin lähettämiseen ja vastaanottamiseen Microsoft 365:n ulkopuolella. Analyysimme osoittaa, että yksi tai useampi ulkoinen sähköpostilähde tai -kohde, jonka olet määrittänyt postin virtauksen yhdistimissä, ei hyväksy yhteyksiä [tässä](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)näkyviltä IP-osoitealueilta.

Toimi ennen 26.10. [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Lisätietoja tästä muutoksesta on ohjeaiheessa Message Centerin viestit [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)tai [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Huomautus:** Jos käytit aiemmin IP- tai URL-osoitteiden julkaisemista HTML-, XML- ja RSS-muodossa päätepistepäivityksiä varten, sinun on myös siirryttävä uusiin verkkopalveluihin tämäntyyppisten päivitysten automatisoimiseksi. Lisätietoja on [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)ohjelm.
