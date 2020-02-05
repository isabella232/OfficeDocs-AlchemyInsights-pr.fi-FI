---
title: Ryhmän lisääminen SharePoint-sivustoon
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: e7bfabe1555bb94e915f8544d460deecce6171be
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770348"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Ongelmia luotaessa ryhmä yhdistettyä sivustoa SharePointissa

1. Joitakin yleisiä ongelmia, joita ilmeni luotaessa tai luotaessa uudelleen ryhmän yhdistettyä sivustoa.
Jos olet poistanut ryhmän ja sen yhdistetyn sivuston ja haluat luoda toisen sivuston, jolla on sama URL-osoite, sinun on poistettava edellinen sivusto pysyvästi.

   - Lataa [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Lisä tietoja PowerShellin käytön aloittamisesta on Ohje aiheessa [SharePoint Onlinen hallinta liittymän käytön](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)aloittaminen.
   - Poista sivusto poistetut sivustot käyttämällä [Poista-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell cmdlet. PowerShell on pakollinen poistamaan ryhmä sivustoja pysyvästi.

1. Jos olet luomassa ryhmä liitettyä sivustoa ja saat varoituksen: **toinen samanniminen ryhmä on jo olemassa**, tarkista olemassa olevat ryhmät [Office 365-sivustosta hallinta keskuksesta](https://admin.microsoft.com/AdminPortal/Home#/groups). Voit ratkaista ongelman poistamalla aiemmin luodun ryhmän, jos sitä ei enää tarvita, tai luomalla sivuston, jossa on eri alias määritetty.

1. On olemassa erilaisia tapoja luoda ja käyttää nykyaikaisia SharePoint-ryhmiä.

   - Voit yhdistää aiemmin luotuja sivustoja Office 365-ryhmään. Lisä tietoja on Ohje aiheessa [Office 365-ryhmän yhdistäminen SharePoint-käyttö liittymän avulla](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Jos haluat luoda Office 365-ryhmään liitetyn sivuston, sinun on luotava [ryhmäsivusto](https://admin.microsoft.com/sharepoint).
