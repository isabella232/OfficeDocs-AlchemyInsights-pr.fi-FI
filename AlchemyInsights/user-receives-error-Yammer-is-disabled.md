---
title: Käyttäjä saa virheen AADSTS7000112 Yammer on poistettu käytöstä
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198059"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>Käyttäjä saa virheen AADSTS7000112 Yammer on poistettu käytöstä

Jos näyttöön tulee virhe "AADSTS7000112: Application '00000005-0000-0ff1-ce00-00000000000'(Yammer) on poistettu käytöstä", Azure AD:n palvelun pääkohteessa on ongelma. Järjestelmänvalvoja on saattanut poistaa palvelun pääkäyttäjän käytöstä estääkseen Yammerin käytön.

Palvelun pääkohteen poistamista käytöstä ei suositella, ja se voi aiheuttaa lisäongelmia. Lisätietoja tuetusta lähestymistavasta Yammerin käytön estämiseksi on [ohjeaiheessa Yammer-käytön poistaminen käytöstä Microsoft 365 -käyttäjille](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).  

Voit korjata tämän ongelman Azure-portaalissa ja palauttaa Yammerin käyttöoikeudet seuraavasti:

1.  Avaa Azure Active Directory -sivu ja valitse vasemman siirtymisruudun **Hallinta-kohdassa** **Yrityssovellukset.**
3.  Kirjoita hakuruutuun **Office 365 Yammer** ja avaa asetukset valitsemalla sovelluksen nimi.
4.  Valitse vasemman siirtymisruudun **Hallinta-kohdassa** **Ominaisuudet.**
5.  Määritä **käytössä-arvoksi Käytössä, jotta käyttäjät voivat kirjautua sisään?** **Yes** **Save**
6.  Kirjaudu Yammeriin uudelleen. Sinun on ehkä tyhjennettävä evästeet.

Voit myös määrittää arvon suorittamalla PowerShell-komentoja. Lisätietoja on [ohjeaiheessa "Anteeksi, mutta sisäänkirjautumisessa on ongelmia" -virhe, kun napsautat Office 365:n Yammer-ruutua.](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365) 