---
title: Useat käyttäjät eivät näe apuosia Outlookissa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197974"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Useat käyttäjät eivät näe apuosia Outlookissa

Jos testaat Outlookin apuohjelmia, eikä mitään näy ensimmäisenä vianmääritysvaiheena, käytä **Get-OrganizationConfig** PowerShell -cmdlet-komentoa _AppsForOfficeEnabled-parametrin_ kyselyyn. Jos kysely palauttaa arvon **False**, määritä tämän parametrin arvoksi **Tosi** **Set-OrganizationConfig-cmdlet-nännin** avulla, joten apuohjelmat näkyvät odotetulla tavalla.

Emme suosittele, että _AppsForOfficeEnabled-parametrin_ arvo on **False**. **False-arvo** ohittaa kaikki edellä mainitut hallinta- ja käyttäjärooliasetukset ja estää organisaation käyttäjän aktivoimasta uusia sovelluksia.

Lisätietoja on [ohjeaiheessa Outlookin apuohjelmia asennettavien ja hallitsevien järjestelmänvalvojien ja käyttäjien määrittäminen](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).