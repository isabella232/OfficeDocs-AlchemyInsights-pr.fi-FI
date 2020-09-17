---
title: 929 Saapuneet-kansion säännöt, joiden avulla voit tyhjentää siirto säännöt
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
- "929"
- "1800021"
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: abb729c40fb87bcca8cc03c95aa4677597d20c08
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47778688"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="f10b6-102">Postin kulku säännöt (tunnetaan myös nimellä siirto säännöt)</span><span class="sxs-lookup"><span data-stu-id="f10b6-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="f10b6-103">Sähkö postin kulku sääntöjen yleisyleiskatsaus: [postin kulku säännöt (siirto säännöt) Exchange Onlinessa](https://technet.microsoft.com/library/jj919238.aspx)</span><span class="sxs-lookup"><span data-stu-id="f10b6-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>

- <span data-ttu-id="f10b6-104">Sähkö postin työn kulku sääntöjen määrittäminen: [sähkö postin kulun säännön toiminto sarjat Exchange Onlinessa](https://technet.microsoft.com/library/dn600436.aspx)</span><span class="sxs-lookup"><span data-stu-id="f10b6-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>

- <span data-ttu-id="f10b6-105">Sähkö postin kulku sääntöjen luominen, muokkaaminen ja poistaminen: [sähkö postin kulku sääntöjen hallinta](https://technet.microsoft.com/library/jj657505.aspx)</span><span class="sxs-lookup"><span data-stu-id="f10b6-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>

<span data-ttu-id="f10b6-106">Voit hallita sähkö postin kulun sääntöjä myös Exchange Online PowerShellissä.</span><span class="sxs-lookup"><span data-stu-id="f10b6-106">You can also manage mail flow rules in Exchange Online PowerShell.</span></span> <span data-ttu-id="f10b6-107">Lisä tietoja on kohdassa [Get-transportrulle](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (Näytä), [Uusi-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (Luo) [, Poista-transportrulle](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (Poista), [Määritä-Transportrulle](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (Muokkaa olemassa olevaa), [Poista-transportrulle](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (Poista olemassa oleva) ja [Enable-transportrulle](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (Ota käyttöön olemassa oleva).</span><span class="sxs-lookup"><span data-stu-id="f10b6-107">For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span>

<span data-ttu-id="f10b6-108">Sähkö postin kulun säännön muut cmdlet-komento: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (luettelon käytettävissä olevat toiminnot), [Get-Transportruclepredikaatti](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (luettelon käytettävissä olevat ehdot ja poikkeukset), [Export-](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) transportrurecollection (vienti säännöt) ja [Import-transportruleccollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (Import rules).</span><span class="sxs-lookup"><span data-stu-id="f10b6-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span>
