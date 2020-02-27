---
title: Luo sähköposti saalis kaikki
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286107"
---
# <a name="create-an-email-catch-all"></a>Luo sähköposti saalis kaikki

Saaliin käyttö kaikki on erittäin suositeltavaa. On parempi antaa kimpsää lähettäjälle, jotta lähettäjät tietävät, että heidän viestiäei voitu toimittaa, jotta he voivat toimia. Voit myös rajoittaa valvotun postilaatikon vain kiinni aiemmin kelvollisia sähköpostiosoitteita. 

Kaikki saalis kaikki postilaatikko saa paljon roskapostia ja voi lopulta täyttää, jos ei tarkasti seurattava. (Raja-arvoja vastaanotetaan.) 

Jos päätät jatkaa, toimi seuraavasti:

1. Luo dynaaminen jakeluryhmä, & sisältää "Kaikki vastaanottajatyypit".

2. Luo oma postilaatikko, jossa voit esimerkiksi catchall@domain.com.

3. Määritä tietylle toimialueelle DomainType-arvoksi InternalRelay. Jos poistat saaliin myöhemmin, muista asettaa toimialueen takaisin arvovaltaiseksi.

4. Luo postivulähetyksen kuljetussääntö seuraavasti:

    - Jos lähettäjä on "Organisaation ulkopuolella"
    - Ohjaa viesti uudelleen Catchall@domain.com
    - Paitsi jos vastaanottaja on allusers@domain.com jäsen (jakeluryhmä sisältää kaikki jäsenet)
    - Varmista, että dynaamiseen jakeluryhmään lisätään uusia postilaatikoita
