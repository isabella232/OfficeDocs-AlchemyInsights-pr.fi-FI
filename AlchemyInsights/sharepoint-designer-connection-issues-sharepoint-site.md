---
title: SharePoint Designer-yhteysongelmat
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 1d3f6ad3128292a9dbcc46cc7da23af59a63fbb4
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840548"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer-yhteysongelmat 

Jos SharePoint Designer on ilmennyt ongelmia yhteyden SharePoint-sivustoihin, yritä seuraavia yhteisiä ratkaisuja.

Vaihe 1: Varmista, että SharePoint Designer 2013 päivitetään [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ja [2. elokuuta 2016 päivittää SharePoint Designer-2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Vaihe 2: Poista tiedostot paikalliseen välimuistiin:

1. Sulje SharePoint Designer-2013.

2. Paikallisen tietokoneen poistaa kaikki tiedostot löytyvät seuraavista kansioista.

    - %APPDATA%\Microsoft\Web palvelimen Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Avaa SharePoint Designer 2013 ja tili uudelleen ja katso jos se toimii.

Vaihe 3: [käyttöön Nykyaikainen Office 2013 laitteissa Windows-todennuksen](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

Vaihe 4: Järjestelmänvalvojien on **Mukautetun komentosarjan avulla** SharePoint-hallintakeskukseen asetukset SharePoint Designer-yhteys. Katso [Salli tai estä mukautetun komentosarjan](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) lisätietoja.


