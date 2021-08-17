---
title: 1554 Winsock-virhe 10061
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
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083227"
---
# <a name="winsock-error-10061"></a>Winsock-virhe 10061

Tämä virhekoodi tarkoittaa, että Microsoft ei pystynyt muodostamaan TCP-vastaketta (yhteyttä) kohde isäntään. Tämän virheen todennäköisin syy on ongelma palomuurin määrityksessä. Voit korjata ongelman tarkistamalla seuraavat asetukset:

- Vahvista palomuurin määritykset [URL-Microsoft 365 ja IP-osoitealueiden tietojen avulla](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Jos virhe koskee Exchange Online Protection (EOP), sinulle olisi pitänyt aiemmin ilmoittaa ip-osoitteiden [Exchange Online Protection muutoksista.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

- Varmista, että Internet-palveluntarjoajasi (ISP) ei estä porttia.

- Vahvista yhdistimien älykkään isännän ja kohdepalvelimen asetukset.

Huomaa, Microsoft 365 ei estä *saapuvia* yhteyksiä tällä tavalla.
