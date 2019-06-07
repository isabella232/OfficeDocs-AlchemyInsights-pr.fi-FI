---
title: Käyttöoikeustasoja SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760690"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer-yhteysongelmat 

Jos SharePoint Designer on ilmennyt ongelmia yhteyden SharePoint-sivustoihin, yritä seuraavia yhteisiä ratkaisuja.

Vaihe 1: Tarkista SharePoint Designer on päivitetty.

- [SharePoint Designer-2013](https://www.microsoft.com/download/details.aspx?id=35491)

- [SharePoint Designerin Service Pack 1 (SP1)](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [Päivitä SharePoint Designer-2013 (KB3114721)](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

Vaihe 2: Poista tiedostot paikalliseen välimuistiin

- Sulje SharePoint Designer-2013.

- Selaa paikallisessa tietokoneessa, voit poistaa välimuistiin tallennetut tiedostot seuraaviin kansioihin.

- Valitse Käynnistä, suorita ja poista kaikki tiedostot löytyy jokaisesta kohdasta sijainteihin alla.

Palvelimen %APPDATA%\Microsoft\Web Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

Avaa SharePoint Designer 2013 ja tili uudelleen ja katso jos se toimii.

Vaihe 3: [käyttöön Nykyaikainen Office 2013 laitteissa Windows-todennuksen](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)

Vaihe 4: Järjestelmänvalvojat on mukautetun komentosarjan avulla voit sallia yhteyden SharePoint Designer.

Saat yksityiskohtaisia ohjeita ja esimerkkejä huomioon otettavia seikkoja [Salli tai estä mukautetun komentosarjan](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


