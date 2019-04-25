---
title: 929 deflectTransport sääntöjä Saapuneet-kansion säännöt
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/15/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 929
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: 880f4cb2c42a564362ad7832ebf8ced16fd26d77
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32413648"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a>Postisääntöjen virtaus (liikenteen säännöt)

- Postisääntöjen virtauksen yleiskatsaus: [postin flow säännöt (Siirtosäännöt) Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)

- Asetukset sähköpostin työnkulkusäännöt: [postin flow säännön menettelyt Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)

- Luoda, muokata ja poistaa sähköpostin työnkulkusäännöt: [Hallitse postisääntöjen vuo](https://technet.microsoft.com/library/jj657505.aspx)

Voit myös hallita Exchange Online PowerShellin yhdistäminen työnkulkusäännöt. Lisätietoja [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (näkymä) [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (luominen), [Poista-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (DEL), [Aseta-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (Muokkaa nykyistä), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (poista aiemmin), ja [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (käyttöön nykyinen).

Uusia työnkulun säännön cmdlet-komennot: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (luetteloon käytettävissä olevat toiminnot), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (luetteloon käytettävissä olevat ehdot ja poikkeukset), [Vie-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (vienti säännöt) ja [ Tuo-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (Tuo säännöt).
