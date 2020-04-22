---
title: Käytön rajoittaminen SharePointissa tai OneDrivessa
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692762"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Käytön rajoittaminen SharePointissa tai OneDrivessa

SharePoint Onlinen ja OneDrive-palveluiden käyttöä voi rajoittaa monella tavalla. Nämä erilaiset käyttörajoitukset on kuvattu alla. 

**Käyttöoikeuksien rajoitus**

SharePoint Onlinessa ja OneDrive for Businessissa rajoitamme sivustojen, tiedostojen ja kansioiden kaltaisten kohteiden käyttöä myöntämällä käyttöoikeuden vain niille ryhmille/henkilöille, joilla pitäisi olla käyttöoikeus.

- [SharePoint-luettelon tai -kirjaston käyttöoikeuksien mukauttaminen](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [SharePoint-sivuston käyttöoikeuksien mukauttaminen](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Alikansion käyttöoikeuksien muuttaminen](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Hallitsemattomien laitteiden käytön hallinta](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

SharePointina tai yleisenä järjestelmänvalvojana voit estää tai rajoittaa SharePoint- ja OneDrive-sisällön käyttöä hallitsemattomista laitteista (jotka eivät ole Intunen yhdistettyjä tai yhteensopivia hybridi-AD:tä).

**Verkon sijainnin rajoitus**

IT-järjestelmänvalvojana voit hallita SharePoint- ja OneDrive-resurssien käyttöä luotettavien määritettyjen verkkosijaintien perusteella. Tätä kutsutaan myös sijaintiin perustuvaksi käytännöksi. Lisätietoja on ohjeaiheessa [SharePoint Online- ja OneDrive-tietojen käytön hallinta verkkosijainnin perusteella](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Sivuston lukituksen rajoitus** 

SharePoint Onlinessa voit lukita sivustokokoelman, joten kenelläkään ei ole käyttöoikeuksia. Tämä määritetään PowerShellin ja [SharePoint Online -hallintaliittymän](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) kautta [Set-SPOSite -LockState-ominaisuuden](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) avulla.

**Käyttäjien estäminen luomasta sivustoja tai alisivustoja**

SharePoint-järjestelmänvalvojana tai yleisenä järjestelmänvalvojana voit antaa käyttäjien luoda ja hallita omia SharePoint-sivustojaan, määrittää, millaisia sivustoja he voivat luoda, ja määrittää sivustojen sijainnin. Lisätietoja on [ohjeaiheessa Sivuston luomisen hallinta SharePoint Onlinessa](https://docs.microsoft.com/sharepoint/manage-site-creation)

