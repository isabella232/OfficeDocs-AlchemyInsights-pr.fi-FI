---
title: Valmistelupalvelun määrittäminen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: 271ab7ad34c0f85f6f5a9d8d3dc2d901fe6fe8f978a2cc98eed986f594036f17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033275"
---
# <a name="configuring-the-provision-service"></a>Valmistelupalvelun määrittäminen

Jotta automaattinen käyttäjien valmistelu toimii, Azure AD edellyttää kelvollisia tunnistetietoja, joiden avulla se voi muodostaa yhteyden Workday-verkkopalveluiden ohjelmointirajapintaan. Lisäksi Workday to AD User Provisioning -sovelluksen Testaa yhteyttä -painike vahvistaa myös, jos se pystyy muodostamaan yhteyden Azure AD Näyttöyhteys-toimialueeseen liittyvään provisioning-agenttiin.

Jos Azure-portaali palauttaa virheen tunnistetietojen tallentamisen yhteydessä, noudata seuraavia suositeltuja ohjeita:

1. Varmista, että olet määrittänyt Workday Integration System -käyttäjätilin opetusohjelman osiossa Integrointijärjestelmän [käyttäjän määrittäminen Työpäivässä mukaisesti.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
2. Varmista, että Azure AD Näyttöyhteys Provisioning Agent Service -palvelu on käytössä paikallisella palvelinpalvelimella Windows hallintakonsolia käyttäen. Voit myös tarkistaa palveluedustajan tilan Azure-portaalissa napsauttamalla Näytä paikalliset edustajat -painiketta.
3. Varmista, että kirjoitat Työpäivänimi-kentän arvon käyttämällä username@workday-vuokraaja-nimi. Jos työpäivä-vuokraajan nimi puuttuu, Työpäivä-todennus epäonnistuu.
4. Jos määrität integroinnin Työpäivä-toteutuksen vuokraajan kanssa, ota huomioon työpäiväsi vuokraajan ajoitetut käyttökatkotunnit. Työpäivä on ajoitettu käyttöajainnille viikonloppuisin (yleensä perjantai-illasta lauantaiaamuun) ja yhteysongelmat tämän käyttökatkosikkunan aikana on tunnettu ongelma, joka ratkaisee automaattisesti heti, kun käyttöönotto vuokralaiset ovat taas online-tilassa.
5. Joissakin harvoissa tapauksissa saatat nähdä tämän virheen myös, jos integrointijärjestelmän käyttäjän salasana muuttuu vuokraajan päivityksen vuoksi tai jos tili on lukittu tai vanhentunut. Tarkista Integrointijärjestelmä-käyttäjän tila Työpäivä-järjestelmänvalvojalta.

Lisätietoja automaattisen valmistelun työpäivän määrittämisestä on kohdassa [Opetusohjelma: Työpäivän määrittäminen automaattista käyttäjien valmistelua varten.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
