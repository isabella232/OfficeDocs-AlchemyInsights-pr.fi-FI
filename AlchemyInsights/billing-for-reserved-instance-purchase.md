---
title: Laskutus varatun esiintymän ostosta
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 00565470de388165e64c45879c22fd5064b4adc695151edaf58878f38a481ff2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104017"
---
# <a name="billing-for-reserved-instance-purchase"></a>Laskutus varatun esiintymän ostosta

Varatun esiintymän hankinta veloitetaan tilaukseen sidottuna olevalla maksutavalla, jonka valitsit ostohetkellä. Tilaustyypin on oltava Enterprise Agreement (tarjousnumero: MS-AZR-0017P), käytön mukaan laskutettava tilaus (tarjousnumero: MS-AZR-0003P), Microsoftin asiakassopimus tai CSP.

- Enterprise-tilauksen maksut veloitetaan rahallisen sitoumuksen saldosta tai ylimaksuna
- Käytön mukaan laskutettavassa tilauksessa maksut laskutetaan tilauksen luottokortti- tai laskumaksulla.

**Varauksen peruminen**

- **Itsepalvelu:** Voit peruuttaa tai vaihtaa varatun tapauksen itse käyttämällä [Azure-portaalia](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Valitse varaus ja sitten hyvitä tai vaihda. Huomaa, että sinulla on oltava omistajan oikeudet varaustilauksessa, jotta voit vaihtaa tai hyvittää varauksen. Pääsy vain varaukseen ei anna sinun jatkaa hyvitystä tai vaihtoa. Pyydä varaustilauksen omistajaa antamaan sinulle omistajan oikeudet varaustilaukseen.
- **Vaihtokäytäntö:** Voit vaihtaa varauksen toiseen samantyyppiseen varaukseen – varauksen voi vaihtaa **seuraamuksetta**. Uuden varauksen kokonaissitoumuksen on oltava suurempi kuin vaihdetun varauksen hyvitysmäärän ja tulevien kuukausimaksujen summa (jos käytössä)
- **Hyvityskäytäntö:** Hyvityksen ja peruuntuneiden tulevien maksujen summa voi olla enintään 50 000 Yhdysvaltain dollaria 12 kuukauden aikana. Tällä hetkellä **emme peri sakkoa** hyvityksistä, mutta voimme periä sitä tulevista palautuksista

**Poikkeukset:** Itsepalveluna tehty vaihto- ja peruutusmahdollisuus ei ole saatavilla Yhdysvaltain hallituksen yrityssopimusasiakkaille.

- **API- / PS- / CLI**-tuki ei ole saatavilla peruutuksiin ja palautuksiin [Azure-varauksien itsepalveluvaihto ja -palautus](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Itsepalveluna tehty vaihto- ja peruutusmahdollisuus ei ole saatavilla Yhdysvaltain hallituksen yrityssopimusasiakkaille. Muut Yhdysvaltain hallituksen tilaustyypit ovat tuettuja, mukaan lukien Pay-As-You-Go ja CSP.

Lisätietoja: [Palautus- ja vaihtotapahtumien](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) käsitteleminen Lisätietoja: Exchange [ja](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) hyvityskäytännöt Muut kysymykset: [Tutustu varattuihin esiintymä-tiedostoihin](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Olemassa olevan varatun tapahtuman vaihtaminen (Itsepalvelu)**

Voit vaihtaa varauksen toiseen samantyyppiseen varaukseen. Voit myös hyvittää varauksen, joka on enintään 50 000 Yhdysvaltain dollaria vuodessa, jos et enää tarvitse sitä. Itsepalveluna tehty vaihto- ja peruutusmahdollisuus ei ole saatavilla Yhdysvaltain hallituksen yrityssopimusasiakkaille. Muut Yhdysvaltain hallituksen tilaustyypit ovat tuettuja, mukaan lukien Pay-As-You-Go ja CSP. Huomaa, että sinulla on oltava omistajan oikeudet varaustilauksessa, jotta voit vaihtaa tai hyvittää varauksen.

Seuraavat vaiheet opastavat toimenpiteen loppuunsaattamisessa

1.Kirjaudu [Azure-portaaliin.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Valitse varaukset, jotka haluat hyvittää, **Exchange** 2.Valitse virtuaalikonetuote, jonka haluat ostaa, ja kirjoita määrä. Varmista, että uusi ostosumma on suurempi kuin palautussumma Määritä oikea [koko ennen ostamista.](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3.Tapahtuman tarkistaminen ja viimeisteleminen

**Varatun tapauksen hyvittäminen**

Jos haluat hyvittää varauksen, siirry kohtaan **Varaustiedot** ja valitse **Hyvitys**

**Suhteutettu tuki**

**Pro ja vähimmäisvaatimusesimerkkejä hyvitystä ja vaihtoa varten** Esimerkki etukäteen varauksesta:

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

**Edellisen laskutusjakson laskua ei voi nähdä**

Joitakin mahdollisia syitä, joiden vuoksi et ehkä näe laskua:

- Sinulla on kuukausittaisen saldon määrä tilauksessasi, jonka ylitit tai jonka olet saanut maksuttomasta kokeiluversiosta. Lasku luodaan vain, kun velkasi on
- Azuren tilauspäivä on alle 30 päivän päässä
- Laskua ei ole vielä luotu. Odota laskutusjakson loppuun asti
- Jos et ole tilin järjestelmänvalvoja, vanhemmat laskut eivät ehkä ole käytettävissäsi

**Lataa laskuSi Azure-portaalista (.pdf)**

- Valitse tilauksesi [Azure-portaalin](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Tilaukset-sivulta [käyttäjänä, jolla on pääsy laskuihin](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Valitse **laskut**
- Valitse **Lataa lasku**, jos haluat nähdä kopion PDF-laskusta. Jos näet **Ei saatavilla** -ilmoituksen, tutustu artikkeliin [Miksi en näe laskua viimeiseltä laskutuskaudelta?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Laskun vastaanottaminen sähköpostitse (.pdf)**

- Valitse tilauksesi [Tilaukset-sivulta.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Valitse **Laskut** ja lähetä lasku sähköpostitse
- Valitse **Ota käyttöön** ja hyväksy ehdot. Sinun on osallistut kuhunkin tilaukseen, jonka omistat

Huomautus: Jos et saa sähköpostiviestiä vaiheiden jälkeen, varmista, että sähköpostiosoitteesi on oikea profiilisi [viestintäasetuksissa.](https://account.windowsazure.com/profile)

**Käyttötietojen lataaminen Azure-portaalista**

- Kirjaudu [Azure-tilikeskukseen](https://account.windowsazure.com/Subscriptions) tilin [järjestelmänvalvojana](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Valitse tilaus, jonka lasku- ja käyttötiedot haluat
- Valitse **laskutushistoria**
- Valitsemalla **Näytä nykyinen lauseke** näet arvion kuluistasi arvion luomisen yhteydessä.
- Lataa **päivittäiset** käyttötiedot CSV-tiedostona valitsemalla Lataa käyttö. Jos näet kaksi versiota saatavilla, lataa versio 2

Muita kysymyksiä: [Katso varattujen tapausten asiakirja](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Suositellut asiakirjat**

- [Laskutuksen perusteet](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Tietoja varatun esiintymän alennuksen alennuksesta](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure-laskutuslaskun ja päivittäisten käyttötietojen lataaminen tai tarkasteleminen](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Tietoja varatun esiintymän alennuksen alennuksesta](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Tietoja Pay-As-You-Go -tilauksesi varatun esiintymän käytöstä](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Enterprise-rekisteröinnin varatun esiintymän käytön ymmärtäminen](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows ohjelmistokustannukset, jotka eivät sisälly varattuihin esiintymään](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Varatut esiintymät Partner Central Pilviratkaisujen toimittaja (CSP) -ohjelmassa](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)