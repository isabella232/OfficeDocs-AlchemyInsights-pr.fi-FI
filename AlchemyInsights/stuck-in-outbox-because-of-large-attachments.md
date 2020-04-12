---
title: Jumissa Lähtevät-kansiossa suurten liitteiden vuoksi
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
- "9002385"
- "4645"
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232627"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Lähtevät-kansioon jumissa olevien viestien korjaaminen

Microsoft suosittelee, että aloitat suorittamalla ongelman sisältävän koneen [Microsoftin tuki- ja palautusavustajatyökalun](https://diagnostics.office.com/#/) [skenaarion "Minulla on ongelmia sähköpostiviestien lähettämisessä, vastaanottamisessa tai etsimisen](https://aka.ms/SaRA-OutlookSendReceive) etsinnässä".

Kun viesti juuttuu Lähtevät-kansioon, todennäköisin syy on suuri liite tai "Lähetä heti, kun yhteys" -vaihtoehto ei ole käytössä.

**Suuren liitteen irrottaminen**

1. Valitse **Lähetä tai vastaanota** > **työ offline-tilassa**. 
2. Valitse siirtymisruudussa **Lähtevät**. Täältä voit: 
    - Poista viesti. Valitse se ja valitse **Poista**.
    - Vedä viesti **luonnoskansioon,** avaa viesti kaksoisnapsauttamalla sitä ja poista liite (napsauta sitä ja valitse **Poista**).
3. Jos virhe ilmoittaa, että Outlook yrittää lähettää viestin, sulje Outlook. Se voi kestää hetken poistua. Jos Outlook ei sulkeudu, paina **Näppäinyhdistelmää Ctrl+Alt+Delete** ja valitse **Käynnistä Tehtävienhallinta**. Valitse Tehtävienhallinnassa **Prosessit-välilehti,** vieritä alas outlook.exe-tiedostoon ja valitse **Lopeta prosessi**.
4. Kun Outlook sulkeutuu, käynnistä Outlook uudelleen ja toista vaiheet 2-3. 
5. Kun olet poistanut liitteen, poista painikkeen valinta ja jatka työskentelyä verkossa valitsemalla **Lähetä tai vastaanota** > **offline-tila.** 

Viestit juuttuvat myös Lähtevät-kansioon, kun valitset **Lähetä**, mutta et ole yhteydessä. Valitse **Lähetä tai vastaanota** ja katso **Offline-tila-painiketta.** Jos se on sininen, yhteys katkeaa. Muodosta yhteys napsauttamalla sitä (painike muuttuu valkoiseksi) ja valitse **Lähetä kaikki**.
 
**Ota lähetä käyttöön heti, kun yhteys on muodostettu**
 
1. Valitse Tiedosto-välilehdessä **Asetukset**.

2. Valitse Outlookin asetukset -valintaikkunassa **Lisäasetukset**.

3. Ota Lähetä heti, **kun yhteys on muodostettu,** valitsemalla Lähetä ja vastaanota -osassa . Valitse **OK**.
 
Lisätietoja on kohdassa:
- [Video: Jumittun sähköpostin lähettäminen tai poistaminen](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [Sähköposti pysyy Lähtevät-kansiossa, kunnes käynnistät lähetys- ja vastaanottotoiminnon manuaalisesti Outlookissa](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
