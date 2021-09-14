---
title: Postilaatikon vastaanottavan rajoituksen pakotus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/31/2021
ms.locfileid: "59315902"
---
# <a name="mailbox-receiving-limit-enforcement"></a>Postilaatikon vastaanottavan rajoituksen pakotus

Microsoft on hiljattain aloittanut postilaatikoita kohden -raja-arvon, joka on 3600 viestiä tunnissa. Lisätietoja on kohdassa Exchange Online [rajoitukset.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits) Microsoft 365 yli 3 600 viestiä tunnissa saapuneiden postilaatikoiden kuormittunutta 60 minuutin ajan. 

Lisäksi lähettäjän ja vastaanottajan parit (OVH) rajoittavat tietyn lähettäjän Microsoft 365 viestit otetaan käyttöön. Jos yksittäinen lähettäjä lähettää tietylle vastaanottajalle yli 33 prosenttia kokonaisrajasta tai 1200 viestiä yhtä vierittämistuntia kohden, OVH-rajoitus tulee käyttöön eikä postilaatikko enää vastaanota viestejä tietyltä lähettäjältä. Huomaa, että:

- Tämä raja on sovellus sähköposteihin, jotka on vastaanotettu muulta vuokrahenkilöltä, paikallisilta lähettäjiltä tai Internet-lähettäjiltä.
- Sähköpostin toimittaminen postilaatikkoon estetään seuraavan 60 minuutin ajaksi. 
- Näiden postilaatikoiden lähettäjät saavat ilmoituksen toimituksen jäyksestä (5.2.121 tai 5.2.122), jossa todetaan, että postilaatikko on ylittänyt toimituksen raja-arvon. Vuokraaja (saman vuokraajan sähköposti) toimitetaan edelleen.
- Kun OVH-raja on käytössä, vastaanottava postilaatikko hyväksyy edelleen viestejä toisilta lähettäjiltä.

Järjestelmänvalvojat voivat valvoa postilaatikon nykyistä toimintaa käyttämällä uutta raporttia ja Exchange hallintakeskuksessa "Postilaatikot, jotka ylittävät vastaanottorajat". Tiedot näkyvät vain, jos vuokraaja on loukkaanut postilaatikoita, kun taas raportti näkyy aina koontinäytössä, mutta on tyhjä, ellei vuokraaja ole loukkaanut postilaatikoita.

Lisätietoja tietojen vastaanottamisen rajoituksista on kohdassa Postilaatikot, jotka ylittävät rajoja koskevat tiedot [uudessa EAC:ssä.](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights)

Lisätietoja ylittävien vastaanottorajoitusten raportista on kohdassa Postilaatikot, jotka ylittävät [vastaanottorajat -raportin uudessa Exchange-valvontaraportissa.](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report)