---
title: Sähkö posti viestin luominen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712983"
---
# <a name="create-an-email-catch-all"></a>Sähkö posti viestin luominen

Kaikkien saaliiden käyttöä ei suositella. On parempi antaa lähettäjälle palautetta siitä, että lähettäjä saa viestin, että hänen viestinsä ei voitu toimittaa niin, että he voivat ryhtyä toimiin. Voit myös rajoittaa valvotun posti laatikon koskemaan vain aiemmin kelvollisia Sähkö posti osoitteita. 

Kaikki saalis kaikki posti laatikot saavat paljon roska postia ja saattavat lopulta täyttyä, jos ne eivät tarkkaan valvo. (Saat rajoituksia.) 

Jos päätät jatkaa, toimi seuraavasti:

1. Luo dynaaminen jako ryhmä, & sisällyttää kaikki vastaanottajatyypit.

2. Luo oma posti laatikko sähkö postien pyytämisestä, esimerkiksi catchall@domain.com.

3. Määritä tietylle toimi alueelle DomainType-asetukseksi "intern Relay". Jos poistat kaikki saalis-asetukset myöhemmin, varmista, että toimi alue määritetään takaisin tärkeiksi.

4. Luo Mailflow-siirto sääntö seuraavasti:

    - Jos lähettäjä on "organisaation ulkopuolinen"
    - Viestin uudelleenohjaus Catchall@domain.com
    - Paitsi, jos edunsaaja on allusers@domain.com-jäsen (Distribution Group sisältää kaikki jäsenet)
    - Varmista, että uudet posti laatikot lisätään dynaamiseen jakeluun-ryhmään
