---
title: 1554 Winsock-virhe 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7651effc43cb0c4bc2fbbe5349bb72303943f493
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32419977"
---
# <a name="winsock-error-10061"></a>WINSOCK-virhe 10061

Tämä virhekoodi tarkoittaa sitä, että Office 365 ei voinut muodostaa TCP socket (yhteys) tavoite isännän kanssa. Tämän virheen Todennäköisin syy on ongelma palomuurin määrityksissä. Voit korjata ongelman, tarkista nämä asetukset:

- Tietoja [Office 365: n URL-osoitteet ja IP-osoitealueita](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges) palomuurin asetusten tarkistaminen

- Jos virhe liittyy, Exchange Online Protection (EOP), sinun olisi aiemmin ilmoitettu muutos [Exchange Online Protection IP-osoitteet](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Varmista, että Internet-palveluntarjoajan (ISP) Estä portti.

- Tarkista smart isäntä- ja palvelimen asetukset yhdistimet.

Huomaa, että Office 365 ei estä *saapuvat* yhteydet tällä tavalla.
