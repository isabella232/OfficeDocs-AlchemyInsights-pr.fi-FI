---
title: Vianmääritys Access estetty viestien OneDrive Business sivustot
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 42a56b17e41649d979cf442909e8357eb262cf9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/28/2019
ms.locfileid: "35354794"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Vianmääritys Access estetty viestien OneDrive Business sivustot

Tämä ongelma ilmenee usein, kun käyttäjä poistetaan ja luodaan uudelleen sama käyttäjätunnus (UPN) kanssa. Uusi tili on luotu käyttämällä eri PUID (yksilöllisen Passport-tunnus)-arvoa. Kun käyttäjä yrittää käyttää sivustokokoelman tai niiden OneDrive, käyttäjällä on virheellinen PUID. Toinen tilanne liittyy directory-synkronointia Active Directoryn organisaatioyksikössä (OU). Jos käyttäjät ovat jo kirjautuneena SharePoint-ovat siirretään eri OU ja SharePointin kanssa resynced, he saattavat kohdata tämän ongelman.

Voit ratkaista tämän ongelman olisi palauttaa alkuperäisen UPN kanssa artikkelin,[Palauta Office 365-käyttäjä](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Tämän jälkeen voit tarkistaa käyttäjällä on admin oikeudet OneDrive-sivuston [admin Lisää käyttäjän, käyttäjän OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive) ohjeiden mukaisesti

Lisätietoja käyttöoikeustasoista on artikkelissa, [ymmärtäminen käyttöoikeustasoja SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
