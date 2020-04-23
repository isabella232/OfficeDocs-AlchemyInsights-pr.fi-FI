---
title: 1554 Winsock virhe 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766166"
---
# <a name="winsock-error-10061"></a>Winsock-virhe 10061

Tämä virhekoodi tarkoittaa, että Microsoft ei voinut muodostaa TCP-vastake (yhteys) kohdeisännän kanssa. Tämän virheen todennäköisin syy on palomuurin kokoonpanoon liittyvä ongelma. Voit korjata ongelman tarkistamalla seuraavat asetukset:

- Tarkista palomuurimääritykset Microsoft [365:n URL-osoitteiden ja IP-osoitealueiden](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges) tiedoilla

- Jos virhe liittyy Exchange Online Protectioniin (EOP), exchange [online protection -IP-osoitteiden](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)muutoksesta olisi pitänyt ilmoittaa aiemmin.

- Varmista, että Internet-palveluntarjoajasi ei estä porttia.

- Tarkista yhdistimien älykkään isännän ja kohdepalvelimen asetukset.

Huomaa, että Microsoft 365 ei estä *saapuvia* yhteyksiä tällä tavalla.
