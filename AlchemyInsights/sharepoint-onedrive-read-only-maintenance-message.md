---
title: Ylläpito viestin vain luku-tilassa, kun yrität käyttää SharePointia tai OneDrivea
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670829"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Ylläpito viestin vain luku-tilassa, kun yrität käyttää SharePointia tai OneDrivea

Käyttäjät voivat saada **vain luku-tilassa olevan ylläpito** viestin, kun he yrittävät käyttää SharePointia tai OneDrivea jossakin seuraavista tilanteista. 

-   Suunniteltu tai aktiivinen huolto toiminto.  Tarkista ne siirtymällä [viesti keskukseen](https://portal.office.com/adminportal/home#/messagecenter).
-   Erittäin tärkeä, aktiivinen palvelu häiriö, joka saattaa olla käynnissä. Tarkista kaikki varoitukset/häiriöt siirtymällä kohtaan [palvelun kunto](https://portal.office.com/adminportal/home#/servicehealth).
-   Pieni automaattisen paranemisen palautus skenaario, joka voi johtua sellaisista palvelimista, jotka saattavat kestää alle 30 minuuttia. 
    
    Näiden vähäisten palautuksista ei ole viesti keskusta tai palvelun kunnon viestejä, mutta sinun pitäisi palata normaaliin hyvin pian.

Olemme havainneet, että yksi edellä mainituista kolmesta skenaarioista on ollut syynä ja että palvelu on palautettu, mutta käyttäjät-selaimen väli muistia ei ole selvitetty.

Yritä tyhjentää selaimen väli muisti ennen sivustoon siirtymistä.

1. Valitse Microsoft Edge-selaimessa **Asetukset**ja valitse sitten **tieto suoja ja suojaus**.
2. Valitse **Tyhjennä selaaminen**-kohdassa **Valitse, mitä haluat tyhjentää**.
3. Valitse **eväs teet ja tallennetut sivuston tiedot**ja valitse **Tyhjennä**.

>[!Note] 
> Nämä vaiheet voivat vaihdella, kun käytät muita selaimia, kuten Mozilla Firefoxia tai Google Chromea.

>[!Note] 
> Toinen vaihto ehto on avata SharePoint-sivusto tai OneDrive uudessa InPrivate-ikkunassa.