---
title: 2491 ilmoitus sähköpostiviestit Phish toimitetaan vuokralaisen tai käyttäjän korvaa käytännön
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391244"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Ilmoitus sähköpostiviestit Phish toimitetaan vuokralaisen tai käyttäjän korvaa käytännön

Oletusarvon mukainen ilmoitus käytännön nimeltä ”käyttäjän tai vuokralaisen ohituksen vuoksi Phish toimitettu” on on rullattu vuokralaiset käyttöoikeudet Office 365-ATP-P1 ja P2. Jos olet saanut ilmoituksen, tässä on vaiheita voit tutkia:

1. Varoitussanoma klikkaa **Näytä ilmoitus** Go to Security & Compliance Centeriin **ilmoitukset** -sivulle.

2. Valitse **näkymässä viestiluettelon** tai **Resurssienhallinnan Näytä viestit**näet ilmoituksen. Nämä asetukset löytyvät tiedot viestin, joka sisältää sanoman tunnus. Huomaa, että uhka Explorer-linkin suodattaa automaattisesti ilmoituksen ehdot täyttävät viestit. Uhka Explorerissa Pvm-suodatus on ehkä muutettava.

Tietojen kalastelu-viesti toimitettiin manuaalisesti määritetty ohituksen vuoksi:

- Sallittu lähettäjän tai toimialueen käyttäjän määrittämä.

- Sallittu lähettäjän tai toimialueen admin Anti-Spam-käytännön mukaan.

- Sallittu käytännössä yhteyden suodattimen IP-osoite.

- Postin kulkua sääntö (tunnetaan myös nimellä liikenteen sääntö), joka on määritetty sallimaan viestien.

Jos viesti on merkitty virheellisesti kalastella, Outlookin avulla [raporttisanoma apuohjelma](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) lähettää viestin Microsoft näytteiden.
