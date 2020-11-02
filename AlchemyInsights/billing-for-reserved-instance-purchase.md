---
title: Varattua esiintymä ostoa laskutetaan
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 6cdcb5af27a475cc838eb434ff025eb18356360c
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823073"
---
# <a name="billing-for-reserved-instance-purchase"></a>Varattua esiintymä ostoa laskutetaan

Varatun esiintymän osto veloitetaan maksu tavasta, joka on sidottu osto hetkellä valitsemaksesi tila ukseen. Tilaus tyypin on oltava Enterprise Agreement (tarjous numero: MS-AZR-0017P), pay-as-you-go (tarjous numero: MS-AZR-0003P), Microsoftin asiakas sopimus tai CSP.

- Jos kyseessä on Enterprise-tilaus, maksut vähennetään rekisteröimisen raha sitoumus saldosta tai veloitetaan ylikautena.
- Pay-as-you-go-pakettina maksut laskutetaan tila uksen luotto kortilla tai laskulla maksu tavalla.

**Vara uksen peruuttaminen**

- **Omatoiminen:** Voit peruuttaa tai vaihtaa varatun esiintymän itse [Azure-portaalin](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)avulla. Valitse varaus ja valitse sitten hyvitys tai Exchange. Huomaa, että sinulla on oltava omistajan käyttö oikeus varaus tilaukseen, jotta voit vaihtaa tai hyvittää. Vain vara uksen käyttäminen ei anna sinun jatkaa hyvitystä tai vaihtaa. Kysy varaus tilauksen omistajalta, jotta voit käyttää varaus tilausta.
- **Exchange-käytännöt:** Voit vaihtaa vara uksen toiseen samantyyppiseen vara uksesta – vara uksen vaihdosta ei **peritä rangaistuksia** . Uuden vara uksen kokonaismäärän on oltava suurempi kuin vaihdettujen varausten palautus summa ja tulevien kuukausittaisten maksujen summa (tarvittaessa).
- **Hyvitys käytännöt:** Hyvityksen summa ja peruutetut tulevat maksu suoritukset eivät saa ylittää $50 000 USD 12 kuukauden rullaava ikkuna. Emme veloita **tällä hetkellä** hyvityksistä, vaan se voi veloittaa tulevista hyvityksistä.

**Poikkeukset:** Omatoiminen Exchange-ja Peruuta-toiminto ei ole käytettävissä Yhdysvaltain hallituksen Enterprise Agreement-asiakkaille

- **API/PS/CLI** -tuki ei ole käytettävissä peruutuksissa ja Hyvityksissa [Itsepalvelupörssien ja Azure-varausten hyvityksille](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support) .
- Omatoiminen Exchange-ja Peruuta-toiminto ei ole käytettävissä Yhdysvaltain hallituksen Enterprise Agreement-asiakkaille. Muita Yhdysvaltain hallituksen tilaus tyyppejä, mukaan lukien pay-as-you-go ja CSP, tuetaan

Lisä tietoja: [palautus-ja Exchange-tapahtumien käsitteleminen](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) lisä tietoja: [Exchange-ja hyvitys käytännöt](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) muut kysymykset: [käy varattuja esiintymä tiedostoja](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Aiemmin luodun varatun esiintymän (Itsepalvelupalvelun) vaihtaminen**

Voit vaihtaa vara uksen toiseen samantyyppiseen vara uksesta. Voit myös hyvittää vara uksen, jopa $50 000 USD vuodessa, jos et enää tarvitse sitä. Omatoiminen Exchange-ja Peruuta-toiminto ei ole käytettävissä Yhdysvaltain hallituksen Enterprise Agreement-asiakkaille. Muita Yhdysvaltain hallituksen tilaus tyyppejä, kuten pay-as-you-go ja CSP, tuetaan. Sinulla on oltava omistajan käyttö oikeus varaus tilauksessa, jotta voit vaihtaa tai hyvittää olemassa olevan vara uksen.

Seuraavat vaiheet opas tavat tapahtuman suorittamiseen.

1. Kirjaudu sisään Azure- [portaaliin](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Valitse hyvitykseen haluamasi vara ukset ja valitse sitten **Exchange** 2. Valitse se VM-tuote, jonka haluat ostaa, ja kirjoita määrä. Varmista, että uusi osto summa on suurempi kuin palautus summa, joka [määrittää oikean koon ennen ostamista](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3. Tarkista ja Viimeistele tapahtuma

**Varatun esiintymän hyvitys**

Jos haluat hyvittää vara uksen, siirry **varaus tiedot** -kohtaan ja valitse **hyvitys** .

**Pro-luokiteltu hyvitys:**

**Pro-annoksesta ja minimi vaatimus esimerkkejä hyvitykseen ja vaihtoon** Etukäteen-varaus esimerkki:

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

**Viimeisen laskutus ajan laskua ei näy**

Mahdollisia syitä siihen, miksi et ehkä näe laskua:

- Sinulla on tilaamasi kuukausittaisen saldon summa, jota et ole ylittänyt tai jossa sinulla on maksuttomat kokeilu versiot. Lasku luodaan vain, kun olet velkaa rahaa
- Se on alle 30 päivää siitä päivästä, kun olet tilannut Azuren
- Laskua ei ole vielä luotu. Odota laskutus vaiheen päättymistä
- Jos et ole tilin ylläpitäjä, Vanhat laskut eivät ehkä ole käytettävissäsi

**Laskun lataaminen Azure-portaalista (. pdf)**

- Valitse tilaus Azure Portal- [tila ukset](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) -sivulta käyttäjänä, [jolla on käyttö oikeus laskuihin](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Valitse **laskut**
- Valitse **Lataa lasku** , jos haluat nähdä kopion PDF-laskusta. Jos se **ei ole käytettävissä** , Katso lisä tietoja kohdasta [Miksi en näe laskua viimeisellä laskutus kaudelta?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Laskun saaminen sähköpostitse (. pdf)**

- Valitse tilaus tila [ukset](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) -sivulla. Valitse **laskut** ja lähetä sähkö postia laskulle
- Valitse **Ilmoittaudu** ja hyväksy ehdot. Sinun on valittava jokaisesta omistamaksustasi

Huomautus: Jos et saa Sähkö posti viestiä noudattamalla ohjeita, varmista, että sähkö posti osoitteesi on oikein [profiilisi viestintä asetuksissa](https://account.windowsazure.com/profile) .

**Käyttö tietojen lataaminen Azure-portaalista**

- Kirjautuminen Azure- [tili keskukseen](https://account.windowsazure.com/Subscriptions) [tilin](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa) järjestelmänvalvojana
- Valitse tilaus, josta haluat laskun ja käyttö tiedot
- Valitse **laskutus historia**
- Valitse **Näytä nykyinen lauseke** , jos haluat nähdä arvion maksuista arvion luonnin yhteydessä.
- Lataa päivittäiset käyttö tiedot CSV-tiedostona valitsemalla **Lataa käyttö** . Jos näet kaksi versiota saatavilla, Lataa versio 2

Muita kysymyksiä: [käy varattuja esiintymä tiedostoja](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Suositellut asia kirjat**

- [Laskutuksen perustiedot](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Miten varattua esiintymä alennusta käytetään?](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure-laskutus laskun ja päivittäisten käyttö tietojen lataaminen tai tarkasteleminen](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Miten varattua esiintymä alennusta käytetään?](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Pay-as-you-go-tila uksen varatun esiintymä käytön ymmärtäminen](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Yrityksen rekisteröinnin varatun esiintymän käytön ymmärtäminen](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows-ohjelmiston kustannukset, jotka eivät sisälly varattuihin esiintymiin](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Varatut esiintymät kumppanien keskitetyn pilvi ratkaisujen tarjoajan (CSP) ohjelmassa](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)