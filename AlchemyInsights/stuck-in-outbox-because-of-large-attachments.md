---
title: Juuttunut Lähtevät-kansioon suurten liitteiden vuoksi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441303"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Lähtevät-kansioon juuttuneen viestin korjaaminen

Microsoft suosittelee, että aloitat suorittamalla skenaarion ["Minulla on ongelmia Sähkö posti viestien lähettämisessä, vastaanottamisessa tai etsimisessä"](https://aka.ms/SaRA-OutlookSendReceive) [Microsoftin tuki-ja palautus avustaja](https://diagnostics.office.com/#/) työkalussa.

Kun viesti juuttuu Lähtevät-kansioon, todennäköiset syyt ovat seuraavat:
- Suuret liitteet.
- **Lähetä heti, kun yhteys on muodostettu** -vaihto ehto ei ole käytössä.

Suurten liitteiden poistaminen: 

1. Valitse Outlookissa **Lähetä tai vastaanota** > **työ offline-tilassa**. 
2. Valitse siirtymis ruudussa **lähtevät-ruutu**. Täältä voit: 
    - Poista viesti (valitse se ja valitse sitten **Poista**).
    - Vedä viesti Luonnokset-kansioon, avaa se kaksoisnapsauttamalla sitä ja poista liite valitsemalla se ja valitsemalla sitten **Poista**).
3. Jos näyttöön tulee virhe sanoma, jonka mukaan Outlook yrittää välittää viestiä, Sulje Outlook. Poistuminen voi kestää hetken. Jos Outlook ei sulkeua, paina Ctrl + Alt + Delete ja valitse **Käynnistä Tehtävienhallinta**. Valitse Tehtävienhallinnassa **prosessit** -väli lehti, Vieritä alaspäin Outlook. exe-kohtaan ja valitse **Lopeta prosessi**.
4. Kun Outlook sulkeutuu, käynnistä se uudelleen ja toista vaiheet 2 ja 3. 
5. Kun olet poistanut liitteen, Jatka työskentelyä verkossa valitsemalla **Lähetä tai vastaanota** > **offline-tilassa** . 

Viestit jäävät myös Lähtevät-kansioon, kun napsautat **Lähetä**-painiketta, mutta et ole yhteydessä. Valitse **Lähetä tai vastaanota** ja katso **työ offline** -painiketta. Jos se on sininen, yhteyteemme katkeaa. Valitse se yhdistääksesi (painike muuttuu valkoiseksi) ja napsauta **Lähetä kaikki**.
 
Lähetyksen ottaminen käyttöön **heti, kun yhteys on muodostettu**:
 
- Valitse **tiedoston** > **Asetukset** >  **Advanced**.
Valitse **Lähetä ja vastaanota** -osiossa **Lähetä heti, kun yhteys on muodostettu**, ja valitse sitten **OK**.
 
Täydelliset tiedot ovat kohdassa:
- [Video: jumissa olevan sähkö postin lähettäminen tai poistaminen](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [Sähkö posti pysyy Lähtevät-kansiossa, kunnes voit aloittaa lähetys-ja vastaanotto toiminnon manuaalisesti Outlookissa](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
