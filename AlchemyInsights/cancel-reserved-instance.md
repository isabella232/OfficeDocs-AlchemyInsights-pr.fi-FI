---
title: Vara uksen peruuttaminen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003552"
- "6817"
ms.openlocfilehash: 04875e33f07c6d0a4306b3579ef81f2d28c7f506
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807574"
---
# <a name="cancelling-reservation"></a>Vara uksen peruuttaminen

- **Omatoiminen:** Voit peruuttaa tai vaihtaa varatun esiintymän itse [Azure-portaalin](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)avulla. Valitse varaus ja valitse sitten hyvitys tai Exchange. Huomaa, että sinulla on oltava omistajan käyttö oikeus varaus tilaukseen, jotta voit vaihtaa tai hyvittää. Vain vara uksen käyttäminen ei anna sinun jatkaa hyvitystä tai vaihtaa. Kysy varaus tilauksen omistajalta, jotta voit käyttää varaus tilausta.
- **Exchange-käytännöt:** Voit vaihtaa vara uksen toiseen samantyyppiseen vara uksesta – vara uksen vaihdosta ei **peritä rangaistuksia** . Uuden vara uksen kokonaismäärän on oltava suurempi kuin vaihdettujen varausten palautus summa ja tulevien kuukausittaisten maksujen summa (tarvittaessa).
- **Hyvitys käytännöt:** Hyvityksen summa ja peruutetut tulevat maksu suoritukset eivät saa ylittää $50 000 USD 12 kuukauden rullaava ikkuna. Emme veloita **tällä hetkellä** hyvityksistä, vaan se voi veloittaa tulevista hyvityksistä.  
    **Poikkeukset:** Omatoiminen Exchange-ja Peruuta-toiminto ei ole käytettävissä Yhdysvaltain hallituksen Enterprise Agreement-asiakkaille
- **API/PS/CLI** -tuki ei ole käytettävissä peruutuksissa ja Hyvityksissa [Itsepalvelupörssien ja Azure-varausten hyvityksille](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support) .
- Omatoiminen Exchange-ja Peruuta-toiminto ei ole käytettävissä Yhdysvaltain hallituksen Enterprise Agreement-asiakkaille. Muita Yhdysvaltain hallituksen tilaus tyyppejä, mukaan lukien pay-as-you-go ja CSP, tuetaan

Lisä tietoja: [palautus-ja Exchange-tapahtumien käsitteleminen](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Lisä tietoja: [Exchange-ja hyvitys käytännöt](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Muita kysymyksiä: [käy varattuja esiintymä tiedostoja](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Aiemmin luodun varatun esiintymän (Itsepalvelupalvelun) vaihtaminen**

Voit vaihtaa vara uksen toiseen samantyyppiseen vara uksesta. Voit myös hyvittää vara uksen, jopa $50 000 USD vuodessa, jos et enää tarvitse sitä. Omatoiminen Exchange-ja Peruuta-toiminto ei ole käytettävissä Yhdysvaltain hallituksen Enterprise Agreement-asiakkaille. Muita Yhdysvaltain hallituksen tilaus tyyppejä, kuten pay-as-you-go ja CSP, tuetaan. Sinulla on oltava omistajan käyttö oikeus varaus tilauksessa, jotta voit vaihtaa tai hyvittää olemassa olevan vara uksen.

Seuraavat vaiheet opas tavat tapahtuman suorittamiseen.

1. Kirjaudu sisään Azure- [portaaliin](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Valitse palautettavan vara uksen ja valitse **Exchange**
2. Valitse VM-tuote, jonka haluat ostaa, ja kirjoita määrä. Varmista, että uusi osto summa on suurempi kuin palautus summa, joka [määrittää oikean koon ennen ostamista](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy) .
3. Tapahtuman tarkistaminen ja suorittaminen

**Varatun esiintymän hyvitys**

Jos haluat hyvittää vara uksen, siirry **varaus tiedot** -kohtaan ja valitse **hyvitys** .

**Pro-luokiteltu hyvitys:**

**Pro-annoksesta ja minimi vaatimus esimerkkejä hyvitykseen ja vaihtoon**  
Etukäteen-varaus esimerkki:

- Olet ostanut yksivuotisen kauden $120 tammi kuun 1.
- 7. huhtikuuta haluat hyvittää tai vaihtaa tämän vara uksen.
- Koska varaus on ollut 97 päivää, saat (1-97/365) * $120 takaisin. (eli $88,1). Hyvityksistä ei tällä hetkellä peritä rangaistusta
- Jos vaihdetaan, uuden ostoksen pitäisi olla suurempi kuin $88,1
- Hyvityksiin ei tällä hetkellä liity rangaistusta

**Laskutus paketin varaus esimerkki:**

- Ostat yksivuotisen kauden $10 kuukaudessa
- 7. huhtikuuta haluat hyvittää tai vaihtaa tämän vara uksen.
- Viimeisen maksun jälkeen 7 päivää, saat (1-7/31) * $10 takaisin. (eli $7,74)
- Tulevat peruutetut maksu suoritukset ovat $80. Hyvityksistä ei tällä hetkellä peritä rangaistusta
- Tämä peruutus vähentää $87,74 sinulta $50 000-hyvityksen rajasta
- Jos vaihdetaan, uuden oston kokonaisarvon pitäisi olla suurempi kuin $87,74

**Suositellut asia kirjat**

- [Palautus-ja Exchange-tapahtumien käsitteleminen](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Exchange-ja hyvitys käytännöt](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)