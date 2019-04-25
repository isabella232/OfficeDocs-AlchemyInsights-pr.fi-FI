---
title: 1065 EOP heikentämisestä lähtevien IP osoite rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 17beb1722142d94ea05b67ce5ed1f20f8b11375c
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404818"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>EOP lähtevien IP-osoitealueita heikentämisestä.

Havaitsimme mahdollinen ongelma on organisaatio, joka (Jos ei korjata lokakuu 26th, 2018) saattaa katkaista postin kulku tiloissa tai ulkoisiin kohteisiin. Kuin aiemmin toimitettujen IP osoitteen alueen hallinnon yksinkertaistamiseksi olemme kokoamassa Exchange Online Protection (EOP) IP-osoitealueiden, joiden avulla voit lähettää ja vastaanottaa sähköposti-Office 365: n ulkopuolella. Meidän analyysi osoittaa, että vähintään yksi ulkoisen sähköpostin lähteitä tai kohteita, jonka olet määrittänyt sähköpostin kulkua liittimet eivät ole hyväksyminen yhteydet IP osoite alueita näytetään [Tässä](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Toimia ennen kuin lokakuu 26th varmistaakseen, että näitä lähteitä ja kohteita hyväksyy kaikki [julkaistu EOP IP-osoitteet](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)-yhteyksistä.

Lisätietoja tästä muutoksesta on Message Center kirjaa, [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)tai [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Huomautus**: Jos olet aiemmin käyttänyt HTML, XML, RSS ja kautta IP- tai URL-Osoitteen julkaiseminen päätepisteen päivitykset, myös syytä siirtää tällaisia päivityksiä automatisoinnin uusi Internet-palveluihin. Lisätietoja [Office 365: ssä päätepisteen luokat ja Office 365: n IP-osoite ja web-palvelun URL-osoite](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
