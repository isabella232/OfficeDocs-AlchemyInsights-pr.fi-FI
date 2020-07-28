---
title: Useilla objekteilla on sama sähköpostiosoite kuin henkilöllisyydellä
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438930"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Useilla objekteilla on sama sähköpostiosoite kuin henkilöllisyydellä

**Useita objekteja**

Yksi tämän virheen yleisistä syistä ei ole se, että Outlook Web Access -pyyntöä ei voi reitittää oikein, jos useissa objekteissa on sama sähköpostiosoite kuin käyttäjätiteetillä. Voit etsiä nämä objektit suorittamalla seuraavat komennot:

· Get-Vastaanottaja<email address>

· Get-Käyttäjä<email address>

· Get-User <email address> -SoftDeletedUser (Get-User -SoftDeletedUser)

· Ota yhteyttä<email address>

· Get-Postilaatikko <email address> -PublicFolder

· Get-Postilaatikko <email address> -IncludeSoftDeletedMailbox

· Get-Postilaatikko <email address> -InactiveMailboxVain

Voit ratkaista ongelman poistamalla useita objekteja, joilla on sama sähköposti-identiteetti, ja varmistamalla, että on olemassa yksi objekti, jolla on tietty sähköpostitunniste ja että sen vastaanottajatyyppi on UserMailbox.

**Samaa osoitetta käytetään yritys- ja kuluttajapostilaatikoissa**

Toinen syy on se, että samaa osoitetta käytetään yritys- ja kuluttajapostilaatikoissa. Tässä tapauksessa käyttäjän on muutettava ensisijaista kuluttajaaliastaan, kunnes Cafe tukee tätä skenaariota. Tämä on pysyvä virhe, joka ei katoa ilman väliintuloa.

Lisätietoja on [ohjeaiheessa Microsoft-tilin sähköpostiosoitteen tai puhelinnumeron muuttaminen](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).