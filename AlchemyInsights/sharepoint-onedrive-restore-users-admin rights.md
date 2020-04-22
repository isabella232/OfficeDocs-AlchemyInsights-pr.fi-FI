---
title: OneDrive for Business -sivustojen käyttöoikeuksien käytön estämistä koskevien viestien vianmääritys
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a83936acf969926c113b28ceb22b006cdb96e2b4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692798"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>OneDrive for Business -sivustojen käyttöoikeuksien käytön estämistä koskevien viestien vianmääritys

Tämä ongelma ilmenee useimmiten, kun käyttäjä poistetaan ja luodaan uudelleen samalla käyttäjänimellä (UPN). Uusi tili luodaan käyttämällä toista PUID (Passport Unique ID) -arvoa. Kun käyttäjä yrittää käyttää sivustokokoelmaa tai OneDrivea, käyttäjällä on virheellinen PUID-tunnus. Toinen skenaario koskee hakemistosynkronointia Active Directory -organisaatioyksikön kanssa. Jos käyttäjät ovat jo kirjautuneet SharePointiin ja siirretään sitten toiseen organisaatioyhteisöön ja synkronoidaan uudelleen SharePointin kanssa, he saattavat kohdata tämän ongelman.

1. Voit ratkaista tämän ongelman palauttamalla alkuperäisen UPN:n artikkelin ohjeiden mukaisesti, [palauta käyttäjä Microsoft 365 :ssä.](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)
2. Jos et pysty palauttamaan alkuperäistä käyttäjää, poista vanha käyttäjä OneDrive-sivustosta seuraavasti, [poista käyttäjä käyttäjätietoluettelosta](). 
3. Kun tämä on tehty, voit varmistaa, että käyttäjällä on OneDrive-sivuston järjestelmänvalvojan oikeudet, noudattamalla kohdan [Järjestelmänvalvojan lisääminen käyttäjän OneDriveen ohjeita.](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Lisätietoja käyttöoikeustasoista on artikkelissa [Tietoja SharePointin käyttöoikeustasoista](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
