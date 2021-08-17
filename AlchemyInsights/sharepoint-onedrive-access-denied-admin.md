---
title: Käyttö estettyjen viestien vianmääritys
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9acde72f82a27c9f2faa2cf4d0417374aa5a294234da96080dc0498d07639248
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085225"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Käyttö estetty -viestien vianmääritys SharePoint- OneDrive hallintakeskuksessa

Jos saat käyttö estetty -viestin, kun yrität selata Sharepoint/ OneDrive-hallintakeskukseen, varmista, että määrität käyttäjälle [käyttöoikeuden.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Jos käyttäjällä on käyttöoikeus, varmista myös, että käyttäjälle on määritetty järjestelmänvalvojan rooli, [joka](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) voi käyttää hallintakeskuksia.

Tämä ongelma voi ilmetä myös silloin, kun käyttäjä poistetaan ja luodaan uudelleen samalla käyttäjätunnuksilla (UPN). Uusi tili luodaan käyttämällä eri PUID (Passport Unique ID) -arvoa. Kun käyttäjä yrittää käyttää sivustokokoelmaa tai hänen OneDrive, käyttäjällä on virheellinen PUID. Toiseen skenaarioon liittyy hakemistosynkronointi Active Directory -organisaatioyksikön (OU) kanssa. Jos käyttäjät ovat jo kirjautuneet SharePoint ja sitten siirretään toiseen OU:han ja synkronoitu SharePoint, he saattavat kokea tämän ongelman.

Voit ratkaista ongelman palauttamista varten alkuperäisen upnimen artikkelin Käyttäjän palauttaminen [Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)

Huomautus: Jos OneDrive tai SharePoint ei ole useiden käyttäjien käytettävissä, joilla oli aiemmin käyttöoikeus, palvelu voi olla tilapäinen.  [Tarkista palvelun kunto -koontinäyttö](https://portal.office.com/adminportal/home#/servicehealth).


