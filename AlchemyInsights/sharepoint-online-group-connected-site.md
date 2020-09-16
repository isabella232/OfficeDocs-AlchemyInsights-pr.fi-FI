---
title: Ryhmän lisääminen SharePoint-sivustoon
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771197"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Ongelmia luotaessa yhdistetyn sivuston ryhmää SharePointissa

1. Yleisiä ongelmia, joita ilmeni luotaessa tai luotaessa uudelleen ryhmää, joka on yhdistetty sivustoon.
Jos olet poistanut ryhmän ja sen yhdistetyn sivuston ja haluat luoda toisen sivuston, jossa on sama URL-osoite, sinun on poistettava aiempi sivusto pysyvästi.

   - Lataa [SPO-hallinta liittymä](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Lisä tietoja PowerShellin käytön aloittamisesta on Ohje aiheessa [SharePoint Online-hallinta liittymän käytön](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)aloittaminen.
   - Poista sivusto poistetuista sivustot [-toiminnolla Remove-SPODeletedSite PowerShell-cmdlet-](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) komennolla. PowerShellin on pakollinen poistaa ryhmä sivustot pysyvästi.

1. Jos luot ryhmään yhdistetyn sivuston ja saat varoituksen: **toinen ryhmä, jolla on sama alias**, on jo olemassa, tarkista olemassa olevat ryhmät [Microsoft 365-hallinta keskuksesta](https://admin.microsoft.com/AdminPortal/Home#/groups). Jos haluat korjata ongelman, Poista olemassa oleva ryhmä, jos sitä ei enää tarvita, tai luo sivusto, jolle on määritetty eri tunnus.

1. Voit luoda ja käyttää nykyaikaisia ryhmiä SharePointin avulla useilla eri tavoilla.

   - Voit yhdistää olemassa olevat sivustot Microsoft 365-ryhmään. Lisä tietoja on Ohje aiheessa [Microsoft 365-ryhmän yhdistäminen SharePoint-käyttö liittymän avulla](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Jos haluat luoda Microsoft 365-ryhmän yhdistetyn sivuston, sinun on luotava [ryhmäsivusto](https://admin.microsoft.com/sharepoint).
