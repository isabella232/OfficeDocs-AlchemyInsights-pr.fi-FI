---
title: SharePoint Designer-yhteys ongelmat
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727168"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer-yhteys ongelmat 

Jos SharePoint Designerissa on SharePoint-sivuston yhteys ongelmia, kokeile seuraavia yleisiä ratkaisuja.

Vaihe 1: Varmista, että SharePoint Designer 2013 on päivitetty SharePoint [Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ja [2016 SharePoint Designer 2013-päivitys](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Vaihe 2: paikallisten väli muisti tiedostojen tyhjentäminen:

1. Sulje SharePoint Designer 2013.

2. Poista paikallisessa tieto koneessa kaikki tiedostot, jotka löytyvät seuraavista kansioista.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\proxetassembrootcache
    - %USERPROFILE%\AppData Local \ Microsoft\websitecache

3. Avaa SharePoint Designer 2013 ja anna tili uudelleen, jotta näet, toimiiko se.

Vaihe 3: [Ota käyttöön moderni todennus Office 2013-palvelua varten Windows-laitteissa](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Vaihe 4: järjestelmänvalvojien on sallittava SharePoint Designer-yhteyden salliminen **mukautetun komento sarjan** avulla SharePoint-hallinta keskuksen asetuksissa. Lisä tietoja on kohdassa [mukautetun komento sarjan salliminen tai estäminen](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .


