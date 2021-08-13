---
title: Käytön rajoittaminen SharePoint OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: fc6731d5a7747bb4fc8d6cef1b6ac0045d11917d7f97abbb21eea9613b1b1aa2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093822"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Käytön rajoittaminen SharePoint OneDrive

Online-/online-palvelujen SharePoint voidaan rajoittaa monella OneDrive tavalla. Nämä käyttörajoitusmenetelmät on kuvattu seuraavassa. 

**Käyttöoikeuksien rajoitus**

SharePoint Onlinessa ja OneDrive for Business rajoitamme sivustojen, tiedostojen ja kansioiden käyttöoikeuksia myöntämällä käyttöoikeudet vain niille ryhmille/henkilöille, joilla on käyttöoikeus.

- [Luettelon tai SharePoint käyttöoikeuksien mukauttaminen](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Sivuston SharePoint mukauttaminen](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Alikansion käyttöoikeuksien muuttaminen](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Hallitsemattomien laitteiden käytön hallinta](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Yleisenä SharePoint tai yleisenä järjestelmänvalvojana voit estää SharePoint ja OneDrive sisällön käytön hallitsemattomista laitteista (joita ei ole liitetty yhdistelmäympäristöön AD tai jotka eivät ole yhteensopivia Intunessa).

**Verkkosijainnin rajoitus**

IT-järjestelmänvalvojana voit hallita resurssien SharePoint OneDrive määritettyjen verkkosijaintien perusteella. Tätä kutsutaan myös sijaintipohjaiseksi käytännönä. Lisätietoja on kohdassa Verkkosijaintiin [perustuvien SharePoint online- OneDrive hallinta](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Sivuston lukituksen rajoitus** 

SharePoint Onlinessa voit lukita sivustokokoelman, joten kukaan ei voi käyttää sitä. Tämä määritetään PowerShellin ja [online SharePoint liittymän kautta](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) [käyttämällä Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState-ominaisuutta.

**Sivustojen tai alisivustojen luomisen estäminen käyttäjiltä**

Järjestelmänvalvojan SharePoint yleisenä järjestelmänvalvojana voit antaa käyttäjien luoda ja hallita omia SharePoint-sivustojaan, määrittää, millaisia sivustoja he voivat luoda, ja määrittää sivustojen sijainnin. Lisätietoja on kohdassa Sivuston luomisen [hallinta SharePoint Onlinessa](https://docs.microsoft.com/sharepoint/manage-site-creation)

