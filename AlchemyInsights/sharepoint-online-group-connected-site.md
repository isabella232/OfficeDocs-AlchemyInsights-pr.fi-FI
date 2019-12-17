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
ms.openlocfilehash: 14ad9dd094902c85eaf0398c76003cea20ad4c0a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051098"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Ongelmia luotaessa tai ryhmittäessä yhdistettyjä sivustoja SharePoint Onlinessa

Ryhmän yhdistettyä sivustoa luotaessa tai luotaessa uudelleen on ilmennyt muutamia yleisiä ongelmia.

 Jos olet poistanut ryhmän ja sen yhdistetyn sivuston ja haluat luoda toisen sivuston, jolla on sama URL-osoite, sinun on poistettava edellinen sivusto pysyvästi.

Lataa [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Lisä tietoja PowerShellin käytön aloittamisesta on Ohje aiheessa [SharePointin online-hallinta liittymän käytön](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) aloittaminen

Poista sivusto poistetut sivustot käyttämällä [Poista-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell cmdlet.

Jos olet luomassa ryhmä liitettyä sivustoa ja saat varoituksen, toinen samanniminen ryhmä on jo olemassa, Tarkista nykyiset ryhmät [Office 365-sivustosta hallinta keskuksesta](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Voit ratkaista ongelman poistamalla aiemmin luodun ryhmän, jos sitä ei enää tarvita, tai luomalla sivuston, jossa on eri alias määritetty.

On olemassa erilaisia tapoja luoda ja käyttää nykyaikaisia SharePoint-ryhmiä.

Voit yhdistää aiemmin luotuja sivustoja Office 365-ryhmään. Lisä tietoja on Ohje aiheessa [Office 365-ryhmän yhdistäminen SharePoint-käyttäjän Interface-toiminnolla](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Jos haluat luoda Office 365-ryhmään liitetyn sivuston, sinun on luotava Ryhmäsivusto. Lisä tietoja on kohdassa [ryhmäsivuston luominen SharePointissa](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

