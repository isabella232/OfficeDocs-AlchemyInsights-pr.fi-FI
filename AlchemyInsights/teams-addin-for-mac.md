---
title: Teams-apuohjelma Macille
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 1e5f6d66386398ad8600f9383f9f7a1dcf0ce69f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670325"
---
# <a name="teams-add-in-for-mac"></a>Teams-apuohjelma Macille

Jos haluat suorittaa puuttuvien teamsin apuohjelmien vian määrityksen Mac-käyttö järjestelmän käyttäjille, toimi seuraavasti:

**Vaihe 1:** Jos sinulla on paikallisesti käytettävä yhdistelmä vaihto (2016 CU3 tai uudempi), varmista Test-HMA.ps1-työkalun avulla, että moderni yhdistelmä todennus on määritetty oikein. Lisä tietoja on Ohje aiheessa [nykyaikaisen yhdistelmä ympäristön todennus määrityksen vahvistaminen Outlook for iOS:ssä ja Androidissa](https://aka.ms/AA980zq).  

**Huomautus** Käytä UPN-osoite muotoa (esimerkiksi [username@contoso.com](mailto:username@contoso.com)), ei toimi alue \ käyttäjä nimi. Tee näin myös käyttäjille, joilla on Exchange Online-posti laatikot.

**Vaihe 2:** Jos haluat, että käyttäjä siirtyy **Työkalut**-  >  **tiliin**... Outlook for Macissa ja Etsi ja valitse tili. Varmista, että mainittu käyttäjä nimi on UPN-muodossa (esimerkiksi [username@contoso.com](mailto:username@contoso.com)).

**Vaihe 3:** Vahvista, että käyttäjä on lisensoitu Microsoft teams-käyttäjä. Käyttäjällä on oltava käytössä Office 365 for Mac-tilaus, tuote versio 16,24 tai uudempi.