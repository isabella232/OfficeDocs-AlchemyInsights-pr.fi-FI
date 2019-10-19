---
title: Rajoita käyttö oikeuksia SharePointissa tai OneDrivessa
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750661"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Rajoita käyttö oikeuksia SharePointissa tai OneDrivessa

SharePoint Online-ja OneDrive-palveluiden käyttöä voi rajoittaa monella tavalla. Nämä erilaiset käyttö rajoitus menetelmät on kuvattu alla. 

**Käyttö oikeus rajoitus**

SharePoint Onlinessa ja OneDrive for Businessissa rajoitamme sivustojen, tiedostojen ja kansioiden kaltaisten kohteiden käyttöä myöntämällä käyttö oikeudet vain niille ryhmille/henkilöille, joilla pitäisi olla käyttö oikeus.

- [SharePoint-luettelon tai-kirjaston käyttö oikeuksien mukauttaminen](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [SharePoint-sivuston käyttö oikeuksien mukauttaminen](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Alikansion käyttö oikeuksien muuttaminen](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Hallitsemattomien laitteiden käytön hallinta](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Voit estää tai rajoittaa SharePoint-ja OneDrive-sisällön käyttö oikeuksia hallitsemattoman laitteen SharePoint-tai 365 Global-järjestelmänvalvojana (ei-hybridi mainoksissa, jotka on liitetty tai yhteensopiva Intune-palvelussa).

**Verkko sijainnin rajoitus**

IT-järjestelmänvalvojana voit hallita SharePoint-ja OneDrive-resurssien käyttöä luotat määritettyjen verkko sijaintien perusteella. Tätä kutsutaan myös sijaintipohjaisiksi käytännöiksi. Lisä tietoja on kohdassa [Hallitse pääsyä SharePoint Onlineen ja OneDrive-tietoihin verkon sijainnin perusteella](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Sivuston lukitus rajoitus** 

SharePoint Onlinessa voit lukita sivustokokoelman, joten kukaan ei voi käyttää sitä. Tämä asetetaan PowerShellin ja [SharePointin online-hallinta liittymän](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) kautta [Set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate-ominaisuuden avulla.

**Sivustojen tai alisivustojen luomisen käyttäjien rajoittaminen**

SharePoint-järjestelmänvalvojana tai Office 365 Global Adminissa voit antaa käyttäjien luoda ja hallinnoida omia SharePoint-sivustoja, määrittää, millaisia sivustoja he voivat luoda ja määrittää sivustojen sijainnin. Lisä tietoja on kohdassa [sivuston luomisen hallinta SharePoint Onlinessa](https://docs.microsoft.com/sharepoint/manage-site-creation)

