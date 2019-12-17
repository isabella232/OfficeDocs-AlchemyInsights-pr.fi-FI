---
title: Vain luku-ylläpito sanoma yritettäessä käyttää SharePointia tai OneDrivea
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051278"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Vain luku-ylläpito sanoma yritettäessä käyttää SharePointia tai OneDrivea

Käyttäjät saattavat saada **vain luku-tilassa olevan ylläpito** sanoman yrittäessään käyttää SharePointia tai OneDrivea jossakin seuraavista tilanteista. 

-   Suunniteltua tai aktiivista kunnossapitoaktiviteettia.  Tarkista ne siirtymällä [viesti keskukseen](https://portal.office.com/adminportal/home#/messagecenter).
-   Erittäin tärkeä aktiivinen palvelu tapahtuma, joka saattaa olla tapahtumassa. Tarkista mahdolliset neuvot/tapahtumat siirtymällä [palvelun terveyteen](https://portal.office.com/adminportal/home#/servicehealth).
-   Pieni auto-Healing elpyminen skenaario, joka voi tapahtua, koska odottamattomia tapahtumia palvelimet, jotka voivat kestää alle 30 min tai niin. 
    
    Näitä vähäisiä takaisinperintöjä varten ei ole Message Center-tai Service Health-viestejä, mutta sinun pitäisi palata normaaliksi hyvin pian.

Hyvin harvoissa tapa uksissa havaitsimme, että yksi edellä mainituista kolmesta skenaariosta on ollut syynä, ja palvelu on palautettu, mutta käyttäjien selaimen väli muistia ei ole selvitetty.

Yritä tyhjentää selaimen väli muisti ennen navigointia sivustoon.

1. Valitse Microsoft Edge-selaimessa **Asetukset**ja valitse sitten **yksityisyys ja suojaus**.
2. Valitse **Tyhjennä selaus**-kohdassa Valitse, **mitä haluat tyhjentää**.
3. Valitse **eväs teet ja tallennetut verkkosivustotiedot**ja valitse **Tyhjennä**.

>[!Note] 
> Nämä vaiheet saattavat vaihdella käytettäessä muita selaimia, kuten Mozilla Firefox tai Google Chrome.

>[!Note] 
> Toinen vaihto ehto olisi avata SharePoint-sivusto tai OneDrive uuteen InPrivate-ikkunaan.