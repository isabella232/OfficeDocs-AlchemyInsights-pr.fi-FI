---
title: 929 Saapuneet-kansion säännöt, jotka koskevat kuljetussääntöjä
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "929"
- "1800021"
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: 6b6e64c0332a579e8f6132b08f2f89b15eb4de27
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43724589"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="e0261-102">Postin kulkua koskevat säännöt (tunnetaan myös siirtosäännöinä)</span><span class="sxs-lookup"><span data-stu-id="e0261-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="e0261-103">Yleistä postin kulkusäännöistä: [Postin kulkusäännöt (siirtosäännöt) Exchange Onlinessa](https://technet.microsoft.com/library/jj919238.aspx)</span><span class="sxs-lookup"><span data-stu-id="e0261-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>

- <span data-ttu-id="e0261-104">Sähköpostin kulun sääntöjen määrittäminen: [Postin kulusäännön toimintosarjat Exchange Onlinessa](https://technet.microsoft.com/library/dn600436.aspx)</span><span class="sxs-lookup"><span data-stu-id="e0261-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>

- <span data-ttu-id="e0261-105">Postin kulkusääntöjen luominen, muokkaaminen ja poistaminen: [Postin kulkusääntöjen hallinta](https://technet.microsoft.com/library/jj657505.aspx)</span><span class="sxs-lookup"><span data-stu-id="e0261-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>

<span data-ttu-id="e0261-106">Voit myös hallita postin kulkusääntöjä Exchange Online PowerShellissä.</span><span class="sxs-lookup"><span data-stu-id="e0261-106">You can also manage mail flow rules in Exchange Online PowerShell.</span></span> <span data-ttu-id="e0261-107">Lisätietoja on [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) [ohjelm.](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule)</span><span class="sxs-lookup"><span data-stu-id="e0261-107">For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span>

<span data-ttu-id="e0261-108">Muut postin kulkusäännön cmdlet-komennot: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (luettelo käytettävissä olevista toiminnoista), [Get-TransportRulePredikaatti](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (luettelo käytettävissä olevista ehdoista ja poikkeuksista), [Vienti-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (vientisäännöt) ja [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (tuontisäännöt).</span><span class="sxs-lookup"><span data-stu-id="e0261-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span>
