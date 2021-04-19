---
title: Teamsin kirjautumisvirhe AADSTS9000411
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821984"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Teamsin kirjautumisvirhe AADSTS9000411

Kun kirjaudut Microsoft Teamsia, saatat saada virheilmoituksen: Valitettavasti AADSTS9000411 -kirjautumisessa on ongelmia: Pyyntöä ei ole muotoiltu **oikein. Parametri "login_hint" kopioidaan.**

Varmista ongelman ratkaisemiseksi, että Microsoft Teams -asiakasohjelmat on päivitetty. Lisätietoja asiakkaan päivittämisestä on kohdassa [Microsoft Teamsin päivittäminen.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)

Jos asiakasohjelmaa ei jostain syystä voi päivittää, asiakkaan kirjaaminen ulos tyhjentää useimmat välimuistiin tallennetut tiedot. Jos kirjautumisen jälkeen on kuitenkin edelleen ongelmia, sulje Teams ja tyhjennä asiakasvälimuisti seuraavasti:
1. Sulje Microsoft Teams.
2. Siirry kansioon %appdata%\microsoft\teams ja poista kaikki tiedostot.
3. Avaa Microsoft Teams uudelleen.
