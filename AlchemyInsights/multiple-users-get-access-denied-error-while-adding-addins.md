---
title: Useat käyttäjät saavat käyttö estetty -virheen lisättäessä apuosia Outlookissa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423712"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Useat käyttäjät saavat käyttö estetty -virheen lisättäessä apuosia Outlookissa

Voit määrittää, kenellä organisaation järjestelmänvalvojilla on oikeudet asentaa ja hallita Outlookin apuohjelmia. Voit myös määrittää, kenellä organisaation käyttäjillä on oikeus asentaa ja hallita apuohjelmia omaan käyttöönsä.

Lisätietoja on [ohjeaiheessa Outlookin apuohjelmia asentavien ja hallitsevien järjestelmänvalvojien ja käyttäjien määrittäminen](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

Voit varmistaa, että olet määrittänyt käyttöoikeudet käyttäjälle, <Role Name> korvaamalla tarkistettavan roolin nimen ja suorittamalla seuraavan komennon Exchange Online PowerShellissä:

Get-ManagementRoleAssignment -Rooli " <Role Name> " -GetEffectiveUsers

Tässä esimerkissä kerrotaan, miten voit tarkistaa, kenelle olet määrittänyt käyttöoikeudet apuosten asentamiseen organisaation Office-kaupasta.

Powershell

-Rooli "Org Marketplace Apps" -GetEffectiveUsers

Tarkista tulokset Get-ManagementRoleAssignment, Tarkista Tehokkaat käyttäjät -sarakkeen merkinnät.

Yksityiskohtaiset syntaksi- ja parametritiedot ovat kohdassa [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 