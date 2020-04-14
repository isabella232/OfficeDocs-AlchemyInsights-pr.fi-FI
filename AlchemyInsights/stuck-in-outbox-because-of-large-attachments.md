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
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241249"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Lähtevät-kansioon jumissa olevien viestien korjaaminen

Microsoft suosittelee, että aloitat suorittamalla [Microsoftin tuki- ja palautusavustajatyökalun](https://diagnostics.office.com/#/) skenaarion ["Minulla on ongelmia sähköpostiviestien lähettämisessä, vastaanottamisessa tai etsimisen etsinnässä".](https://aka.ms/SaRA-OutlookSendReceive)

Kun viesti juuttuu Lähtevät-kansioon, todennäköisin syy on suuri liite tai "Lähetä heti, kun yhteys" -vaihtoehto ei ole käytössä.

**Suuren liitteen irrottaminen**

1. Valitse Outlookissa **Lähetä tai vastaanota** > **työ offline-tilassa**. 
2. Valitse siirtymisruudussa **Lähtevät**. Täältä voit: 
    - Poista viesti (valitse se ja valitse sitten **Poista**).
    - Vedä viesti Luonnokset-kansioon, avaa se kaksoisnapsauttamalla sitä, poista liite ja valitse se ja valitse sitten **Poista**).
3. Jos näyttöön tulee virhe, jonka mukaan Outlook yrittää lähettää viestin, sulje Outlook. Se voi kestää hetken poistua. Jos Outlook ei sulkeudu, paina Näppäinyhdistelmää Ctrl+Alt+Delete ja valitse **Aloita Tehtävienhallinta**. Valitse Tehtävienhallinnassa **Prosessit-välilehti,** vieritä alas outlook.exe-tiedostoon ja valitse **Lopeta prosessi**.
4. Kun Outlook sulkeutuu, käynnistä se uudelleen ja toista vaiheet 2 ja 3. 
5. Kun olet poistanut liitteen, jatka työskentelyä verkossa valitsemalla **Lähetä tai vastaanota** > **offline-tilassa.** 

Viestit juuttuvat myös Lähtevät-kansioon, kun valitset **Lähetä**, mutta et ole yhteydessä. Valitse **Lähetä tai vastaanota** ja katso **Offline-tila-painiketta.** Jos se on sininen, yhteys katkeaa. Muodosta yhteys napsauttamalla sitä (painike muuttuu valkoiseksi) ja valitse **Lähetä kaikki**.
 
**Ota lähetä käyttöön heti, kun yhteys on muodostettu**
 
1. Valitse Tiedosto-välilehdessä **Asetukset**.

2. Valitse Outlookin asetukset -valintaikkunassa **Lisäasetukset**.

3. Ota Lähetä heti, **kun yhteys on muodostettu,** valitsemalla Lähetä ja vastaanota -osassa . Valitse **OK**.
 
Lisätietoja on kohdassa:
- [Video: Jumittun sähköpostin lähettäminen tai poistaminen](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [Sähköposti pysyy Lähtevät-kansiossa, kunnes käynnistät lähetys- ja vastaanottotoiminnon manuaalisesti Outlookissa](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
