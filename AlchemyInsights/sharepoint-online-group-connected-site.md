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
ms.openlocfilehash: b54457427ffa563b6a6323d85e1c8800191eca11
ms.sourcegitcommit: a98b25fa3cac9ebba983f4932881d774880aca93
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/13/2020
ms.locfileid: "44064390"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Ongelmia luotaessa ryhmään yhdistettyä sivustoa SharePointissa

1. Joitakin yleisiä ongelmia, joita ilmeni luotaessa tai luotaessa uudelleen ryhmään yhdistettyä sivustoa.
Jos olet poistanut ryhmän ja siihen liitetyn sivuston ja haluat luoda toisen sivuston, jolla on sama URL-osoite, sinun on poistettava edellinen sivusto pysyvästi.

   - Lataa [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Lisätietoja Powershellin käytön aloittamisesta on ohjeaiheessa [SharePoint Online Management Shellin käytön aloittaminen](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Poista sivusto poistetuista sivustoista [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell -cmdlet-komennolla. Ryhmäsivustojen poistaminen pysyvästi edellyttää Powershelliä.

1. Jos luot ryhmään yhdistetyn sivuston ja saat varoituksen: **Toinen ryhmä, jolla on sama alias, on jo olemassa,** tarkista aiemmin luodut ryhmät [Microsoft 365 -hallintakeskuksesta](https://admin.microsoft.com/AdminPortal/Home#/groups). Voit ratkaista ongelman poistamalla aiemmin luodun ryhmän, jos sitä ei enää tarvita, tai luomalla sivuston, jolle on määritetty toinen alias.

1. Voit luoda ja käyttää moderneja ryhmiä SharePointin avulla eri tavoilla.

   - Voit yhdistää aiemmin luotuja sivustoja Microsoft 365 -ryhmään. Lisätietoja on [ohjeaiheessa Microsoft 365 -ryhmän yhdistäminen SharePoint-käyttöliittymän avulla](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Jos haluat luoda Microsoft 365 -ryhmään yhdistetyn sivuston, sinun on luotava [ryhmäsivusto](https://admin.microsoft.com/sharepoint).
