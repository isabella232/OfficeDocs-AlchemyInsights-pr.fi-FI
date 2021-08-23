---
title: Haluatko ilmoittaa roskapostiviestistä Virheellisestä roskapostista Microsoftille?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "975"
- "666"
- "3100019"
ms.openlocfilehash: d3897f24ce9a967b08a3fd15a2fdedbb3fe2a22d
ms.sourcegitcommit: f05d4caa0e657ee74d6b6e9abc88488f17d740fe
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/19/2021
ms.locfileid: "58396612"
---
# <a name="do-you-have-legitimate-messages-being-marked-as-spam"></a>Onko luotettavat sähköpostiviestisi merkitty roskapostiksi?

On turhauttavaa, kun aito sähköpostiviesti päätyy Roskaposti-kansioon tai karanteeniin. Ota seuraavat yleisimmät syyt virheellisten positiivisten tietojen tekoon:

**Vuokraajan ohitukset (yleisin)** Tämä on täysin sinun hallinnassasi korjausta varten.

Lähetä viesti Microsoft 365 Defender ja analysoi vaikutuskäytäntöjä ja sääntöjä rescan details are available within minutes.
Tarkastele tai muokkaa käytäntöjä tai sääntöjä tarpeen mukaan. 

**Loppukäyttäjän ohitukset (yleinen)** Tämä on täysin sinun hallinnassasi korjausta varten. 

Lähetä viesti Microsoft 365 Defender ja analysoi vaikutuskäytäntöjä ja sääntöjä rescan details are available within minutes. 

Jos viesti estettiin, koska se on lähetetty käyttäjän Estetyt lähettäjät -luettelossa olevasta osoitteesta, otsikot sisältävät roskapostisuodatusilmoituksen "SFV:BLK".

**Lähettäjien sähköpostin todennus** Tämä korjaus on osittain sinun hallinnassasi.

Lähetä viesti analysoimaan lähettäjän sähköpostitodennuksessa toimitusvirheitä; tulokset ovat saatavilla päivän kuluessa. 

Jos omistat lähettävän infrastruktuurin, tarkista, miten se sovitetaan yhteen SPF-, DKIM- ja DMARC-tietueiden kanssa ja varmista, että kohdesähköpostijärjestelmät luottavat toimialueestasi lähetettyihin viesteihin. Vaihtoehtoisesti voit ottaa yhteyttä lähettäjiin DNS-määritysten osoitteita varten.

**Microsoftin suodatuskomiset** Tämä korjaus on osittain sinun hallinnassasi.

Lähetä viesti ja ilmoita viesti turvalliseksi; uudelleenhaun tulokset ovat saatavilla päivän kuluessa. Käytä vuokraajan sallittujen ja estojen luetteloa, jos et ole eri mieltä ja suodatat päätös saneluja erityisissä tilanteissa. Älä kuitenkaan ohita Microsoftin suodatuskokeiluja pysyvästi. 

Lisätietoja on seuraavissa artikkeleissa:

- Anna loppukäyttäjien lähettää viestejä Microsoftille. Microsoft käyttää näitä ilmoituksia sähköpostin suojaustekniikoiden tehokkuuden parantamiseen, ja ne näkyvät lähetysraporteissa, jotta voit käyttää niitä merkkinä päivityskäytännöistä. 

- Jos haluat katsoa lyhyen videon viestien lähettämisestä analysoimista varten, katso viestien [lähettäminen analyysia varten.](https://go.microsoft.com/fwlink/?linkid=2166435)

- [Järjestelmänvalvojan lähetyksen avulla voit lähettää roskapostia, tietoja, URL-osoitteita ja tiedostoja Microsoftille](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission)

- [Vuokraajan sallittujen ja estettyjen luettelon hallinta](https://docs.microsoft.com/microsoft-365/security/office-365-security/tenant-allow-block-list)

- [Roskapostin estoviestien otsikot Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)

- [Lähtevän roskapostin suojaus EOP:ssä](https://docs.microsoft.com/microsoft-365/security/office-365-security/outbound-spam-controls)