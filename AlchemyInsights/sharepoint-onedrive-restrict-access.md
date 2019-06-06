---
title: Kirjoita SharePoint- tai OneDrive käytön rajoittaminen
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 5101366ff65f477c19b9c7f2c0d7065cf88501b0
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735140"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Kirjoita SharePoint- tai OneDrive käytön rajoittaminen

SharePoint Online/OneDrive palvelujen käytön rajoittaminen monilla tavoilla. Seuraavassa esitetyt menetelmät eri access-rajoitus. 

Käyttöoikeuden rajoittaminen

SharePoint Online-ja liiketoiminnan OneDrive olemme rajoittaa esimerkiksi sivustot, tiedostot ja kansiot vain myöntäminen ryhmiä ja vastaavien käyttäjien olisi päästävä.

[Voit mukauttaa SharePoint-luettelon tai kirjaston käyttöoikeudet](https://support.office.com/en-us/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

[Voit mukauttaa SharePoint-sivuston käyttöoikeudet](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions)

[Muuta alikansion käyttöoikeuksia](https://support.office.com/en-us/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

[Hallitsemattomien laitteiden käytön hallinta](https://docs.microsoft.com/en-us/sharepoint/control-access-from-unmanaged-devices)

SharePoint-tai Office 365: ssä yleisen järjestelmänvalvojan estää tai rajoittaa pääsyä laitteiden hallitsemattomaan SharePoint-ja OneDrive (nämä hybridi liitettyjen tai yhteensopiva Intune AD).

Verkon sijainti rajoittamiseen

IT-järjestelmänvalvojana voit hallita SharePoint- ja OneDrive määriteltyjen verkkosijainteihin, joihin luotat perustuvat resurssien käyttöä. Tätä kutsutaan myös sijaintiin perustuva käytäntö. Lisätietoja on ohjeaiheessa [SharePoint Online ja OneDrive verkkosijaintiin perustuvien tietojen käytön valvonta](https://docs.microsoft.com/en-us/sharepoint/control-access-based-on-network-location)

Sivustorajoitusta lukitus 

Sinulla on mahdollisuus lukita niin, että kukaan pääsee sivustokokoelman sisällä SharePoint Online. Määritä PowerShell- ja [SharePoint Online-hallintaliittymä](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) käyttämällä [Set-SPOSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState-ominaisuuden kautta.

Sivustojen ja alisivustojen luominen estäminen

SharePoint-järjestelmänvalvoja tai yleisen järjestelmänvalvojan Office 365: ssä, voit antaa käyttäjien luoda ja hallinnoida omia SharePoint-sivustot, selvittää, mitä sivustoja he voivat luoda, ja määritä sijainti sivustot. Lisätietoja on kohdassa [Hallitse sivuston luominen SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/manage-site-creation)

