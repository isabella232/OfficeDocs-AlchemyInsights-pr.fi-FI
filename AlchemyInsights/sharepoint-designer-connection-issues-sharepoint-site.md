---
title: SharePoint Design Erin yhteys ongelmat
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051710"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Design Erin yhteys ongelmat 

Jos SharePoint Designerissa ilmenee yhteys ongelmia SharePoint-sivustoissa, kokeile seuraavia yhteisiä ratkaisuja.

Vaihe 1: Varmista, että SharePoint Designer 2013 on päivitetty [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ja [elokuun 2, 2016 päivitys SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Vaihe 2: Tyhjennä paikalliset väli muisti tiedostot:

1. Sulje SharePoint Designer 2013.

2. Poista paikallisesta tieto koneesta kaikki tiedostot, jotka löytyvät kaikista seuraavista kansioista.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Avaa SharePoint Designer 2013 ja anna tili uudelleen nähdäksesi, onko se toimii.

Vaihe 3: [Ota käyttöön moderni todennus Office 2013-laitteille Windows-laitteissa](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

Vaihe 4: järjestelmänvalvojien on **sallittava mukautettu komento sarja** SharePointin hallinta keskuksen asetuksissa, jotta SharePoint Designer-yhteys voidaan sallia. Lisä tietoja on kohdassa [mukautetun komento sarjan salliminen tai estäminen](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .


