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
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481854"
---
# <a name="configuring-the-provision-service"></a>Valmistelupalvelun määrittäminen

Jotta automaattinen käyttäjien valmistelu toimii, Azure AD edellyttää kelvollisia tunnistetietoja, joiden avulla se voi muodostaa yhteyden Työpäivä-verkkopalveluiden ohjelmointirajapintaan. Lisäksi Työpäivä- ja AD-käyttäjien valmistelusovelluksen Testaa yhteyttä -painike vahvistaa myös, jos se pystyy muodostamaan yhteyden AD-toimialueeseen liittyvään Azure AD Connect -valmisteluedustajaan.

Jos Azure-portaali palauttaa virheilmoituksen tunnistetietojen tallentamisen yhteydessä, noudata seuraavia suositeltuja ohjeita:

1. Varmista, että olet määrittänyt Työpäivä-integroinnin järjestelmän käyttäjätilin opetusohjelman kohdassa Määritä [integrointijärjestelmän käyttäjä Työpäivässä.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
2. Varmista, että Azure AD Connect -valmisteluagenttipalvelu on käytössä paikallisella Windows-palvelimella palveluiden hallintakonsolin avulla. Voit tarkistaa edustajan tilan myös Azure-portaalissa napsauttamalla Näytä paikalliset edustajat -painiketta.
3. Varmista, että kirjoitat Työpäivänimi-kentän arvon käyttämällä username@workday vuokraajan nimen muotoilua. Jos työpäivä- ja vuokraajanimi puuttuu, Työpäivä-todennus epäonnistuu.
4. Jos olet määrittämässä integrointia Työpäivä-toteutuksen vuokraajan kanssa, ota huomioon Työpäivä-vuokraajan ajoitetut käyttökatkotunnit. Työpäivä on ajoitettu käyttöajalta viikonloppuisin (yleensä perjantai-illasta lauantaiaamuun) ja yhteysongelmat tämän käyttökatkosikkunan aikana on tunnettu ongelma, joka korjaantuminen automaattisesti heti, kun toteutuksen vuokralaiset ovat taas online-tilassa.
5. Joissakin harvoissa tapauksissa saatat nähdä tämän virheen myös, jos integrointijärjestelmän käyttäjän salasana muuttuu vuokraajan päivityksen vuoksi tai jos tili on lukittuna tai vanhentunut. Tarkista Integrointijärjestelmä-käyttäjän tila Työpäivä-järjestelmänvalvojalta.

Lisätietoja työpäivän määrittämisestä automaattista valmistelua varten on opetusohjelmassa: Työpäivän määrittäminen [automaattista käyttäjien valmistelua varten.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
