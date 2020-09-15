---
title: Käyttö estetty-viestien vian määritys OneDrive for Business-sivustossa
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670613"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Käyttö estetty-viestien vian määritys OneDrive for Business-sivustossa

Tämä ongelma ilmenee useimmiten silloin, kun käyttäjä poistetaan ja luodaan uudelleen käyttäen samaa käyttäjän päänimeä (UPN). Uusi tili luodaan käyttämällä toista PUID (Passport Unique ID)-arvoa. Kun käyttäjä yrittää käyttää sivustokokoelmaa tai OneDrivea, käyttäjällä on virheellinen PUID. Toinen skenaario sisältää hakemisto synkronoinnin Active Directoryn organisaatio yksikön (OU) kanssa. Jos käyttäjä on jo kirjautunut SharePointiin ja siirtyy sitten toiseen organisaatio yksikköön ja on siirretty SharePointiin, ongelma saattaa ilmetä.

1. Voit korjata ongelman palauttamalla alkuperäisen UPN:N artikkelin ohjeiden mukaisesti ja [palauttamalla käyttäjän Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)-sovelluksessa.
2. Jos et pysty palauttamaan alkuperäistä käyttäjää, sinun on poistettava vanha käyttäjä OneDrive-sivustosta noudattamalla näitä ohjeita, [poistamalla käyttäjä käyttäjä tieto luettelosta](). 
3. Kun tämä on tehty, voit tarkistaa, että käyttäjällä on järjestelmänvalvojan oikeudet OneDrive-sivustoon, noudattamalla ohjeita, jotka koskevat [järjestelmänvalvojan lisäämistä käyttäjän OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles) -palveluun.

Lisä tietoja käyttö oikeus tasoista on artikkelissa tietoja [SharePointin käyttö oikeus tasoista](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
