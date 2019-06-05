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
ms.openlocfilehash: 7451cfe957545537298f57feb5b47bd6d43cddbf
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716889"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer-yhteysongelmat 

<p>Jos SharePoint Designer on ilmennyt ongelmia yhteyden SharePoint-sivustoihin, yritä seuraavia yhteisiä ratkaisuja.</p> <p><strong>Vaihe 1:</strong> <strong>Tarkista SharePoint Designer on päivitetty&nbsp; </strong></p> <ul> <li><a href="https://www.microsoft.com/en-us/download/details.aspx?id=35491">SharePoint Designer-2013</a></li> <li><a href="https://support.microsoft.com/en-us/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1">SharePoint Designerin Service Pack 1 (SP1)</a></li> <li><a href="https://support.microsoft.com/en-us/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721">Päivitä SharePoint Designer-2013 (KB3114721)</a></li> </ul> <p><strong>Vaihe 2:</strong> <strong>Poista tiedostot paikalliseen välimuistiin</strong>&nbsp;</p> <ol> <li style="font-weight: 400;">Sulje SharePoint Designer-2013.&nbsp;</li> <li style="font-weight: 400;">Selaa paikallisessa tietokoneessa, voit poistaa välimuistiin tallennetut tiedostot seuraaviin kansioihin.&nbsp;</li> <li style="font-weight: 400;">Napsauta <strong>Käynnistä -&gt; suorittaa</strong> ja poista kaikki tiedostot, löytyy jokaisesta kohdasta sijainteihin alla.&nbsp;<br /><br />%APPDATA%\Microsoft\Web palvelimen Extensions\Cache<br />%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache<br />%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</li> <li style="font-weight: 400;">Avaa SharePoint Designer 2013 ja tili uudelleen ja katso jos se toimii.</li> </ol> <p><strong>Vaihe 3:</strong> <a href="https://docs.microsoft.com/en-us/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=%252fen-us%252farticle%252fEnable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&amp;view=o365-worldwide"> <strong>Käyttöön Nykyaikainen Office 2013 laitteissa Windows-todennuksen</strong></a>&nbsp;</p> <p><strong>Vaihe 4:</strong> <strong>Järjestelmänvalvojien on SharePoint Designer-yhteyden avulla mukautetun komentosarjan</strong>.</p> <p>Saat yksityiskohtaisia ohjeita ja esimerkkejä huomioon otettavia seikkoja <a href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">Salli tai estä mukautetun komentosarjan</a>.&nbsp;</p>


