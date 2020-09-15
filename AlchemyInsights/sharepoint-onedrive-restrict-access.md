---
title: Käytön rajoittaminen SharePointissa tai OneDrivessa
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700452"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Käytön rajoittaminen SharePointissa tai OneDrivessa

SharePoint Online-ja OneDrive-palveluiden käyttöä voi rajoittaa monin eri tavoin. Seuraavat eri käytön rajoitus tavat on kuvattu alla. 

**Käyttö oikeus rajoitus**

SharePoint Onlinessa ja OneDrive for Businessissa rajoitetaan kohteiden, kuten sivuston, tiedostojen ja kansioiden, käyttöä myöntämällä vain niiden ryhmien/henkilöiden oikeudet, joilla on oikeus käyttää niitä.

- [SharePoint-luettelon tai-kirjaston käyttö oikeuksien mukauttaminen](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [SharePoint-sivuston käyttö oikeuksien mukauttaminen](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Alikansion käyttö oikeuksien muuttaminen](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Hallitsemattomien laitteiden käytön hallinta](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

SharePoint-tai yleinen-järjestelmänvalvojana voit estää tai rajoittaa SharePoint-ja OneDrive-sisällön käyttöä hallitsemattomista laitteista (ne, joita ei ole yhdistetty tai jotka on liitetty tai yhteensopiva Intunella).

**Verkko sijainnin rajoitus**

IT-järjestelmänvalvojana voit hallita SharePointin ja OneDriven resurssien käyttöä luotettavien verkko sijaintien perusteella. Tätä kutsutaan myös sijaintiin perustuväksi käytännöksi. Lisä tietoja on Ohje aiheessa [SharePoint Onlinen ja OneDrive-tietojen käytön hallinta verkko sijainnin perusteella](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Sivuston lukitus rajoitus** 

SharePoint Onlinessa sinulla on mahdollisuus lukita sivustokokoelma, joten kukaan ei voi käyttää sitä. Tämä määritetään PowerShellin ja [SharePoint Online-hallinta liittymän](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) kautta käyttämällä [joukkoa-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate-ominaisuutta.

**Sivuston tai alisivuston luomisen rajoittaminen käyttäjille**

Kun olet SharePoint-järjestelmänvalvoja tai yleinen järjestelmänvalvoja, voit antaa käyttäjien luoda ja hallita omia SharePoint-sivustojaan, määrittää, millaisia sivustot voivat luoda ja määrittää sivuston sijainnin. Lisä tietoja on kohdassa [sivuston luomisen hallinta SharePoint Onlinessa](https://docs.microsoft.com/sharepoint/manage-site-creation)

