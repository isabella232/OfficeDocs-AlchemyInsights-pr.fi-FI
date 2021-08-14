---
title: Osoite Teams kirjautumisvirhe AADSTS9000411
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
ms.openlocfilehash: 883bf48d3628702c92361a5250f0d59e1352918349b8bc6c3eae5a948b72fc57
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53953017"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Osoite Teams kirjautumisvirhe AADSTS9000411

Kun kirjaudut Microsoft Teams, näyttöön voi tulla seuraava virhesanoma: Valitettavasti AADSTS9000411 -kirjautumisessa on ongelmia: Pyyntöä ei ole muotoiltu **oikein. Parametri "login_hint" kopioidaan.**

Varmista ongelman ratkaisemiseksi, että asiakas Microsoft Teams päivitetään. Lisätietoja asiakkaan päivittämisestä on kohdassa [Asiakasohjelman Microsoft Teams.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)

Jos asiakasohjelmaa ei jostain syystä voi päivittää, asiakkaan kirjaaminen ulos tyhjentää useimmat välimuistiin tallennetut tiedot. Jos kirjautumisen jälkeen on kuitenkin edelleen ongelmia, sulje Teams ja tyhjennä asiakasvälimuisti seuraavasti:
1. Sulje Microsoft Teams.
2. Siirry kansioon %appdata%\microsoft\teams ja poista kaikki tiedostot.
3. Avaa Microsoft Teams.
