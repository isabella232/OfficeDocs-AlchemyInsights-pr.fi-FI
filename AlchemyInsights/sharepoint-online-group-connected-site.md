---
title: Ryhmän lisääminen SharePoint sivustoon
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 5dd159b8b9e141c2fb448bae5fb624efe1014d7d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318121"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Yleisiä ongelmia luotaessa ryhmää yhdistettyä sivustoa SharePoint

1. Jos olet poistanut ryhmän ja sen yhdistetyn sivuston ja haluat luoda toisen sivuston, jolla on sama URL-osoite, sinun on poistettava edellinen sivusto pysyvästi.

   - [Lataa SPO-hallintaliittymä](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Lisätietoja PowerShellin käytön aloittaminen on kohdassa [Online-hallintaliittymän käytön SharePoint aloittaminen.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)
   - Poista sivusto Poistetut sivustot -komennolla [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell-cmdlet-komennolla. Ryhmäsivustojen poistaminen pysyvästi edellyttää Powershelliä.

1. Jos luot ryhmään yhdistetyn sivuston ja saat varoituksen: Toinen ryhmä, jolla on sama tunnus, on jo olemassa , tarkista aiemmin luodut [ryhmät](https://admin.microsoft.com/AdminPortal/Home#/groups)Microsoft 365 -hallintakeskus . Voit ratkaista ongelman poistamalla aiemmin luodun ryhmän, jos sitä ei enää tarvita, tai luomalla sivuston, jolle on määritetty toinen alias.

1. Nykyaikaisten ryhmien luominen ja käyttö on eri SharePoint.

   - Voit yhdistää aiemmin luodut sivustot Microsoft 365 ryhmään. Katso lisätietoja Näyttöyhteys [ryhmästä Microsoft 365 käyttöliittymän SharePoint avulla.](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)
   - Jos haluat Microsoft 365 ryhmään yhdistetyn sivuston, sinun on luotava [ryhmäsivusto.](https://admin.microsoft.com/sharepoint)
