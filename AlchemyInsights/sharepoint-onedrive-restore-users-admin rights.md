---
title: OneDrive for Business-sivustojen käyttö estetty-sanomien vian määritys
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9d8aba4e53a1e0505a430296bb1c11713ea2ce7b
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051602"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>OneDrive for Business-sivustojen käyttö estetty-sanomien vian määritys

Tämä ongelma ilmenee useimmin, kun käyttäjä poistetaan ja luodaan uudelleen samalla käyttäjä nimellä (UPN). Uusi tili luodaan käyttämällä eri PUID (Passport Unique ID)-arvoa. Kun käyttäjä yrittää käyttää sivustokokoelmaa tai OneDrivea, käyttäjällä on väärä PUID-tunnus. Toinen skenaario koskee hakemiston synkronointia Active Directory-organisaatio yksikön (OU) kanssa. Jos käyttäjät ovat jo kirjauduneet sisään SharePointiin ja ne siirretään toiseen kohteeseen ja synkronoidaan SharePointin kanssa, ongelma saattaa ilmetä.

1. Voit ratkaista tämän ongelman palauttamalla alkuperäisen UPN artikkelin vaiheet, [Palauta käyttäjä Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Jos et pysty palauttamaan alkuperäistä käyttäjää, poista vanha käyttäjä OneDrive-sivustosta näiden vaiheiden avulla, [Poista käyttäjä käyttäjän tiedot-luettelosta](). 
3. Kun tämä on tehty, voit varmistaa, että käyttäjällä on järjestelmänvalvojan oikeudet OneDrive-sivustoon noudattamalla ohjeita, jotka [lisäävät järjestelmänvalvojan tiedot käyttäjän OneDriveen](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Lisä tietoja käyttö oikeus tasoista on artikkelissa [SharePoint-käyttö oikeus tasojen ymmärtäminen](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
