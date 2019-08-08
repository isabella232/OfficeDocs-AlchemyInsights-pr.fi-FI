---
title: Vianmääritys Access estetty viestien OneDrive Business sivustot
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: d47ce80bdd07a25d9724057edf0289808a00a3db
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232521"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Vianmääritys Access estetty viestien OneDrive Business sivustot

Tämä ongelma ilmenee usein, kun käyttäjä poistetaan ja luodaan uudelleen sama käyttäjätunnus (UPN) kanssa. Uusi tili on luotu käyttämällä eri PUID (yksilöllisen Passport-tunnus)-arvoa. Kun käyttäjä yrittää käyttää sivustokokoelman tai niiden OneDrive, käyttäjällä on virheellinen PUID. Toinen tilanne liittyy directory-synkronointia Active Directoryn organisaatioyksikössä (OU). Jos käyttäjät ovat jo kirjautuneena SharePoint-ovat siirretään eri OU ja SharePointin kanssa resynced, he saattavat kohdata tämän ongelman.

1. Voit ratkaista tämän ongelman olisi palauttaa alkuperäisen UPN kanssa artikkelin,[Palauta Office 365-käyttäjä](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Jos et pysty palauttamaan alkuperäinen käyttäjä poistaa vanhan käyttäjän OneDrive-sivuston, näillä ohjeilla, [Poista käyttäjä-käyttäjätietojen luettelossa](). 
3. Tämän jälkeen voit tarkistaa käyttäjällä on admin oikeudet OneDrive-sivuston [admin Lisää käyttäjän, käyttäjän OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive) ohjeiden mukaisesti

Lisätietoja käyttöoikeustasoista on artikkelissa, [ymmärtäminen käyttöoikeustasoja SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
