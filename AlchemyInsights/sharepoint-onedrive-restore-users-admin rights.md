---
title: OneDrive for Business -sivustojen käytön estämien viestien vianmääritys
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 95bd46e8b7a6006f3735612d9a5602fb2b2a283b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511181"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>OneDrive for Business -sivustojen käytön estämien viestien vianmääritys

Tämä ongelma ilmenee useimmiten, kun käyttäjä poistetaan ja luodaan uudelleen samalla käyttäjänimellä (UPN). Uusi tili luodaan käyttämällä toista PUID (Passport Unique ID) -arvoa. Kun käyttäjä yrittää käyttää sivustokokoelmaa tai OneDrivea, käyttäjällä on virheellinen PUID-tunnus. Toinen skenaario koskee hakemistosynkronointia Active Directory -organisaatioyksikön kanssa. Jos käyttäjät ovat jo kirjautuneet SharePointiin ja siirtyvät sitten toiseen organisaatioyksikköön ja synkronoivat sharepointin uudelleen, he saattavat kohdata tämän ongelman.

1. Voit ratkaista tämän ongelman palauttamalla alkuperäisen UPN-numeron artikkelin ohjeiden mukaisesti, [jotka on tarkoitettu käyttäjän palauttamiseen Microsoft 365 :ssä](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Jos et pysty palauttamaan alkuperäistä käyttäjää, poista vanha käyttäjä OneDrive-sivustosta seuraavasti, [poista käyttäjä käyttäjätietoluettelosta](). 
3. Kun tämä on tehty, voit varmistaa, että käyttäjällä on järjestelmänvalvojan oikeudet OneDrive-sivustoon, noudattamalla käyttäjän [OneDrive-järjestelmänvalvojan käyttäjien järjestelmänvalvojan oikeuksien lisäämistä](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Lisätietoja käyttöoikeustasoista on artikkelissa [Tietoja SharePointin käyttöoikeustasoista](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
