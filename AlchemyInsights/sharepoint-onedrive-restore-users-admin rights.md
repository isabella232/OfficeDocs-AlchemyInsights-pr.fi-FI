---
title: Estettyjen sanomien vianmääritys OneDrive for Business sivustoille
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
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957790"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Estettyjen sanomien vianmääritys OneDrive for Business sivustoille

Tämä ongelma ilmenee useimmiten silloin, kun käyttäjä poistetaan ja luodaan uudelleen samalla käyttäjätunnuksilla (UPN). Uusi tili luodaan käyttämällä eri PUID (Passport Unique ID) -arvoa. Kun käyttäjä yrittää käyttää sivustokokoelmaa tai hänen OneDrive, käyttäjällä on virheellinen PUID. Toiseen skenaarioon liittyy hakemistosynkronointi Active Directory -organisaatioyksikön (OU) kanssa. Jos käyttäjät ovat jo kirjautuneet SharePoint ja sitten siirretään toiseen OU:han ja synkronoitu SharePoint, he saattavat kokea tämän ongelman.

1. Voit ratkaista ongelman palauttamaan alkuperäisen upnin käyttäjätunnuksen artikkelin Käyttäjän palauttaminen [Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)
2. Jos et voi palauttaa alkuperäistä käyttäjää, poista vanha käyttäjä OneDrive-sivustosta seuraavasti: Käyttäjän poistaminen [käyttäjätietojen luettelosta.]() 
3. Kun tämä on tehty, voit varmistaa, että käyttäjällä on OneDrive-sivuston järjestelmänvalvojan oikeudet, noudattamalla ohjeita, jotka koskevat järjestelmänvalvojan [OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Lisätietoja käyttöoikeustasoista on artikkelissa Tietoja [käyttöoikeustasoista SharePoint.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)
