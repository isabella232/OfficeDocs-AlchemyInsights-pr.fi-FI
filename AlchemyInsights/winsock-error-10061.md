---
title: 1554 WINSOCK-virhe 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698859"
---
# <a name="winsock-error-10061"></a>WINSOCK-virhe 10061

Tämä virhe koodi tarkoittaa, että Microsoft ei pystynyt muodostamaan TCP-vastaketta (yhteyttä) kohde isäntään. Todennäköisin syy tähän virheeseen on palo muurin määrityksessä oleva ongelma. Jos haluat korjata ongelman, valitse seuraavat asetukset:

- Palo muurin määritysten tarkistaminen [Microsoft 365-URL-osoitteiden ja IP-osoite alueiden](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges) tiedoilla

- Jos virhe on määritetty Exchange Online Protection (ESIP)-palvelussa, sinun olisi pitänyt olla aiemmin ilmoitettu [Exchange Online Protection-IP-osoitteiden](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)muutokseen.

- Varmista, ettei Internet-palveluntarjoajasi estä porttia.

- Varmista, että yhdistimessä on älykäs isäntä-ja kohde palvelin-asetukset.

Huomaa, että Microsoft 365 ei estä *saapuvia* yhteyksiä tällä tavalla.
