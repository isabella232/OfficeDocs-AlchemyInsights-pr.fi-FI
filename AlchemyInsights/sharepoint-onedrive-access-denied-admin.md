---
title: Käytön estämien viestien vianmääritys
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505376"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Access Denied -viestien vianmääritys Sharepointissa/OneDrive-hallintakeskuksessa

Jos saat käyttöestetty -sanoman, kun yrität selata Sharepoint/OneDrive-hallintakeskusta, varmista, että [määrität käyttäjälle käyttöoikeuden.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Jos käyttäjällä on käyttöoikeus, varmista myös, että [hänelle on määritetty järjestelmänvalvojan rooli,](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) joka voi käyttää hallintakeskuksia.

Tämä ongelma voi ilmetä myös silloin, kun käyttäjä poistetaan ja luodaan uudelleen samalla käyttäjänimellä (UPN). Uusi tili luodaan käyttämällä toista PUID (Passport Unique ID) -arvoa. Kun käyttäjä yrittää käyttää sivustokokoelmaa tai OneDrivea, käyttäjällä on virheellinen PUID-tunnus. Toinen skenaario koskee hakemistosynkronointia Active Directory -organisaatioyksikön kanssa. Jos käyttäjät ovat jo kirjautuneet SharePointiin ja siirtyvät sitten toiseen organisaatioyksikköön ja synkronoivat sharepointin uudelleen, he saattavat kohdata tämän ongelman.

Voit ratkaista tämän ongelman palauttamalla alkuperäisen UPN-numeron artikkelin ohjeiden mukaisesti, [jotka artikkelissa Palauta käyttäjä Microsoft 365:ssä](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Huomautus: Jos OneDrive- tai SharePoint-hallintakeskus ei ole käytettävissä useille käyttäjille, joilla on aiemmin ollut käyttöoikeus, saattaa olla tilapäinen palveluongelma.  [Tarkista palvelun kunnon koontinäyttö](https://portal.office.com/adminportal/home#/servicehealth).


