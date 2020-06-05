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
ms.openlocfilehash: 5dab9fce935936898927afd55f8f6e9260249157
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582808"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Ongelmia luotaessa ryhmälle yhdistettyä sivustoa SharePointissa

1. Joitakin yleisiä ongelmia ilmeni luotaessa tai luotaessa uudelleen yhdistettyä ryhmää.
Jos olet poistanut ryhmän ja siihen liittyvän sivuston ja haluat luoda toisen sivuston, jolla on sama URL-osoite, sinun on poistettava edellinen sivusto pysyvästi.

   - Lataa [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Lisätietoja Powershellin käytön aloittamisesta on ohjeaiheessa [SharePoint Online -hallintaliittymän käytön aloittaminen](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Poista sivusto poistetuista sivustoista [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell -cmdlet-nännin avulla. Ryhmäsivustojen poistaminen edellyttää Powershelliä.

1. Jos luot ryhmään yhdistettyä sivustoa ja saat varoituksen: **Toinen ryhmä, jolla on sama alias, on jo olemassa,** tarkista aiemmin luodut ryhmät [Microsoft 365 -hallintakeskuksesta](https://admin.microsoft.com/AdminPortal/Home#/groups). Voit ratkaista ongelman poistamalla aiemmin luodun ryhmän, jos sitä ei enää tarvita, tai luomalla sivuston, jossa on toinen alias määritettynä.

1. Voit luoda ja käyttää moderneja ryhmiä SharePointin kanssa eri tavoin.

   - Voit yhdistää aiemmin luodut sivustot Microsoft 365 -ryhmään. Lisätietoja on [ohjeaiheessa Microsoft 365 -ryhmän yhdistäminen SharePoint-käyttöliittymän avulla](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Jos haluat luoda Microsoft 365 -ryhmän yhdistetyn sivuston, sinun on luotava [ryhmäsivusto](https://admin.microsoft.com/sharepoint).
