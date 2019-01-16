---
title: 1554 Winsock-virhe 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 96a9cfd11941158ddf13655c74974e3eb800e570
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/15/2019
ms.locfileid: "28286621"
---
# <a name="winsock-error-10061"></a>WINSOCK-virhe 10061

Tämä virhekoodi tarkoittaa sitä, että Office 365 ei voinut muodostaa TCP socket (yhteys) tavoite isännän kanssa. Tämän virheen Todennäköisin syy on ongelma palomuurin määrityksissä. Voit korjata ongelman, tarkista nämä asetukset:
  
- Tietoja [Office 365: n URL-osoitteet ja IP-osoitealueita](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges) palomuurin asetusten tarkistaminen
    
- Jos virhe liittyy, Exchange Online Protection (EOP), sinun olisi aiemmin ilmoitettu muutos [Exchange Online Protection IP-osoitteet](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
    
- Varmista, että Internet-palveluntarjoajan (ISP) Estä portti.
    
- Tarkista smart isäntä- ja palvelimen asetukset yhdistimet.
    
Huomaa, että Office 365 ei estä *saapuvat* yhteydet tällä tavalla. 
  

