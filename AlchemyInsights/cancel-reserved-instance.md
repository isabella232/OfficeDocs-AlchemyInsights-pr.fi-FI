---
title: Varauksen peruminen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003552"
- "6817"
ms.openlocfilehash: 8d0a6a37a244e817472c3949109481a30d80328b7353806905e05c547e196ea0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931230"
---
# <a name="cancelling-reservation"></a>Varauksen peruminen

- **Itsepalvelu:** Voit peruuttaa tai vaihtaa varatun tapauksen itse käyttämällä [Azure-portaalia](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Valitse varaus ja sitten hyvitä tai vaihda. Huomaa, että sinulla on oltava omistajan oikeudet varaustilauksessa, jotta voit vaihtaa tai hyvittää varauksen. Pääsy vain varaukseen ei anna sinun jatkaa hyvitystä tai vaihtoa. Pyydä varaustilauksen omistajaa antamaan sinulle omistajan oikeudet varaustilaukseen.
- **Vaihtokäytäntö:** Voit vaihtaa varauksen toiseen samantyyppiseen varaukseen – varauksen voi vaihtaa **seuraamuksetta**. Uuden varauksen kokonaissitoumuksen on oltava suurempi kuin vaihdetun varauksen hyvitysmäärän ja tulevien kuukausimaksujen summa (jos käytössä)
- **Hyvityskäytäntö:** Hyvityksen ja peruuntuneiden tulevien maksujen summa voi olla enintään 50 000 Yhdysvaltain dollaria 12 kuukauden aikana. Tällä hetkellä **emme peri sakkoa** hyvityksistä, mutta voimme periä sitä tulevista palautuksista  
    **Poikkeukset:** Itsepalveluna tehty vaihto- ja peruutusmahdollisuus ei ole saatavilla Yhdysvaltain hallituksen yrityssopimusasiakkaille.
- **API- / PS- / CLI**-tuki ei ole saatavilla peruutuksiin ja palautuksiin [Azure-varauksien itsepalveluvaihto ja -palautus](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Itsepalveluna tehty vaihto- ja peruutusmahdollisuus ei ole saatavilla Yhdysvaltain hallituksen yrityssopimusasiakkaille. Muut Yhdysvaltain hallituksen tilaustyypit ovat tuettuja, mukaan lukien Pay-As-You-Go ja CSP.

Lisätietoja: [Miten palautus- ja vaihtotapahtumat käsitellään](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Lisätietoja: [Vaihto- ja hyvityskäytännöt](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Muita kysymyksiä: [Katso varattujen tapausten asiakirja](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Olemassa olevan varatun tapahtuman vaihtaminen (Itsepalvelu)**

Voit vaihtaa varauksen toiseen samantyyppiseen varaukseen. Voit myös hyvittää varauksen, joka on enintään 50 000 Yhdysvaltain dollaria vuodessa, jos et enää tarvitse sitä. Itsepalveluna tehty vaihto- ja peruutusmahdollisuus ei ole saatavilla Yhdysvaltain hallituksen yrityssopimusasiakkaille. Muut Yhdysvaltain hallituksen tilaustyypit ovat tuettuja, mukaan lukien Pay-As-You-Go ja CSP. Huomaa, että sinulla on oltava omistajan oikeudet varaustilauksessa, jotta voit vaihtaa tai hyvittää varauksen.

Seuraavat vaiheet opastavat toimenpiteen loppuunsaattamisessa

1. Kirjaudu sisään [Azure-portaaliin](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Valitse varaus, jonka haluat hyvittää ja valitse sitten **Vaihda**.
2. Valitse VM-tuote, jonka haluat ostaa ja kirjoita määrä. Varmista, että uuden oston loppusumma on suurempi kuin palautuksen loppusumma [Oikean koon määrittäminen ennen ostamista](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Tarkista ja suorita maksutapahtuma loppuun

**Varatun tapauksen hyvittäminen**

Jos haluat hyvittää varauksen, siirry kohtaan **Varaustiedot** ja valitse **Hyvitys**

**Suhteutettu tuki**

**Esimerkkejä hyvityksen ja vaihtamisen suhteuttamisesta ja vähimmäisvaatimuksista**  
Esimerkki ennakkovarauksesta:

- Ostat yhden vuoden RI:n 120 $:lla tammikuun 1. päivänä
- Huhtikuun 7. päivänä haluat hyvittää tai vaihtaa tämän varauksen
- Koska varaus on ollut voimassa 97 päivää, saat (1-97/365) * 120 $:a takaisin. (eli 88,1 $) Hyvityksistä ei tällä hetkellä peritä sakkoa
- Jos vaihdat, uuden ostoksesi on oltava suurempi kuin 88,1 $:a
- Hyvityksistä ei tällä hetkellä peritä sakkoa

**Esimerkki laskutussuunnitelmalla tehdystä varauksesta:**

- Ostat yhden vuoden RI:n 10 $:lla joka kuukausi
- Huhtikuun 7. päivänä haluat hyvittää tai vaihtaa tämän varauksen
- Koska viimeinen maksu tapahtui 7 päivää sitten, saat (1-7/31) * 10 $:a takaisin. (eli 7,74 $)
- Tulevat peruutetut maksut ovat 80 $:a. Hyvityksistä ei tällä hetkellä peritä sakkoa
- Tämä hyvitys vähentää 87,74 $:a 50 000 $ hyvitysrajasta
- Jos vaihdat, uuden ostoksesi kokonaismäärä on oltava suurempi kuin 87,74 $:a

**Suositellut asiakirjat**

- [Miten palautus- ja vaihtotapahtumat käsitellään](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Vaihto- ja hyvityskäytännöt](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)