---
title: Sähköpostiviestin luominen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 0d20f7bcffa3be43fc6186a938bf4a7338722f5cd225b860da6357398db26a69
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080743"
---
# <a name="create-an-email-catch-all"></a>Sähköpostiviestin luominen

Kaikkien takuiden käyttö ei ole suositeltavaa. On parempi antaa lähettäjälle ilmoitus viestin lähettäjälle siitä, että viestiä ei voitu toimittaa osoitettaan, jotta lähettäjä voi ryhtyä toimenpiteisiin. Voit myös rajoittaa valvotulle postilaatikolle vain aiemmin kelvolliset sähköpostiosoitteet. 

Kaikki kaikki postilaatikot saavat paljon roskapostia, ja ne saattavat täyty, jos niitä ei valvota tarkasti. (Rajoituksia on.) 

Jos haluat jatkaa, toimi seuraavasti:

1. Luo dynaaminen jakeluryhmä, & "Kaikki vastaanottajatyypit".

2. Luo erillinen postilaatikko sähköpostiviestien pyytä varten, esimerkiksi catchall@domain.com.

3. Määritä tietyn toimialueen DomainType-tyypiksi InternalRelay. Jos poistat kaikki toimialueet myöhemmin, muista määrittää toimialue takaisin arvoksi Authoritative.

4. Luo Postinkulku-siirtosääntö seuraavasti:

    - Jos lähettäjä on Organisaation ulkopuolinen
    - Ohjaa viesti Catchall@domain.com
    - Paitsi jos vastaanottaja on jäsen allusers@domain.com (Jakeluryhmä sisältää kaikki jäsenet)
    - Varmista, että uudet postilaatikot lisätään dynaamiseen jakeluryhmään
