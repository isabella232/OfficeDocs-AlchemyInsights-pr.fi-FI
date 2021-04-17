---
title: Varatun esiintymän oston laskutus
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
ms.openlocfilehash: 9d71554d2089a6d9e5d4850149d113959f3d43c0
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820319"
---
# <a name="billing-for-reserved-instance-purchase"></a>Varatun esiintymän oston laskutus

Varatun esiintymän osto veloitetaan maksutavalla, joka on sidottu ostohetkellä valitsemaani tilaukseen. Tilaustyypin on oltava enterprise agreement (offer number: MS-AZR-0017P), Pay-As-You-Go (offer number: MS-AZR-0003P), Microsoft Customer Agreement tai CSP.

- Enterprise-tilauksen maksut vähennetään rekisteröinnin rahamääräinen sitoumussaldo tai veloitetaan ylimaksuna
- Pay-As-You-Go -tilauksen maksut laskutetaan tilauksen luottokortti- tai laskumaksutavalla.

**Varauksen peruuttaminen**

- **Omatoiminen:** Voit peruuttaa tai vaihtaa varatun esiintymän itse [Azure-portaalin avulla.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Valitse varaus ja napsauta hyvitystä tai vaihtoa. Huomaa, että sinulla on oltava varaustilauksen omistajan käyttöoikeudet, jotta voit vaihtaa tai hyvittää tilauksen. Vain varauksen käyttö ei anna sinun jatkaa hyvitystä tai vaihtoa. Pyydä varauksen omistajaa antamaan sinulle varaustilauksen omistajan käyttöoikeudet
- **Exchange-käytäntö:** Voit vaihtaa varaukseen toisen samantyyppisen varauksen – **varauksesta** ei seuraa seuraamuksia. Uuden varauksen kokonaissitoumusten on oltava suurempi kuin vaihdettu varauksesi hyvityssumma ja tulevat kuukausierät (tarvittaessa)
- **Hyvityskäytäntö:** Hyvityksen ja peruutetut tulevat maksut eivät voi ylittää 50 000 Yhdysvaltain dollaria 12 kuukauden juoksevassa ikkunassa. Emme tällä **hetkellä veloita hyvityksistä mitään,** mutta voimme veloittaa sen tulevista hyvityksistä

**Poikkeukset:** Omatoiminen vaihto ja peruutusominaisuus eivät ole saatavilla US Government Enterprise Agreement -asiakkaille

- **API / PS / CLI -tuki** ei ole käytettävissä peruutusta ja hyvitystä varten Omatoiminen vaihto ja [Azure-varauksista hyvitystä](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Omatoiminen vaihto ja peruutusominaisuus eivät ole saatavilla US Government Enterprise Agreement -asiakkaille. Muita Yhdysvaltain julkishallinnon tilaustyyppejä, kuten Pay-As-You-Go- ja CSP-tilaustyyppejä, tuetaan

Lisätietoja: [Palautus- ja](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) vaihtotapahtumien käsitteleminen Lisätietoja : [Exchange-](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) ja Hyvityskäytännöt Muut kysymykset: [Tutustu varattuihin esiintymä-docs-tiedostoihin](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Aiemmin varatun esiintymän exchange(omatoiminen)**

Voit vaihtaa varauksen toisen samantyyppistä varausta varten. Voit myös hyvittää varauksen, joka on enintään 50 000 Yhdysvaltain dollaria vuodessa, jos et enää tarvitse sitä. Omatoiminen vaihto ja peruutusominaisuus eivät ole saatavilla US Government Enterprise Agreement -asiakkaille. Muita Yhdysvaltain valtionhallinnon tilaustyyppejä, kuten Pay-As-You-Go- ja CSP-palvelu, tuetaan. Sinulla on oltava varaustilauksen omistajan käyttöoikeudet, jotta voit vaihtaa tai hyvittää olemassa olevan varauksen.

Seuraavien vaiheiden avulla voit suorittaa tapahtuman loppuun.

1.Kirjaudu [Azure-portaaliin.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Valitse varaukset, jotka haluat hyvittää, ja valitse **Exchange** 2.Valitse virtuaalikonetuote, jonka haluat ostaa, ja kirjoita määrä. Varmista, että uusi ostosumma on suurempi kuin palautussumma Määritä oikea [koko ennen ostamista.](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3.Tapahtuman tarkistaminen ja viimeisteleminen

**Varatun esiintymän hyvitys**

Jos haluat hyvittää varauksen, siirry **Varauksen tiedot -ruudulle** ja valitse **Hyvitys.**

**Hyvitetty hyvitys:**

**Hyvitystä ja vaihtoa koskevat pro-ration- ja vähimmäisvaatimusesimerkkejä** Esimerkki etukäteen varauksesta:

- Ostat yhden vuoden RI-termin hintaan 120 $, kun 1. tammikuuta
- 7. huhtikuuta, haluat hyvittää tai vaihtaa tämän varauksen
- Koska varaus on ollut live-tilassa 97 päivää, saat (1-97/365) * 120 $ takaisin. (88,1 $). Hyvityksistä ei tällä hetkellä ole hyvitystä
- Jos vaihdat, uuden ostoksen pitäisi olla suurempi kuin 88,1 $.
- Tällä hetkellä hyvityksistä ei ole olemassa hyvitystä

**Esimerkki laskutussuunnitelman varauksen varauksesta:**

- Ostat yhden vuoden RI-termin hintaan 10 $ kuukaudessa
- 7. huhtikuuta, haluat hyvittää tai vaihtaa tämän varauksen
- Koska viimeinen maksu on tapahtunut 7 päivää, saat (1-7/31) * 10 $ takaisin. (7,74 $)
- Peruutetut tulevat maksut ovat 80 $. Hyvityksistä ei tällä hetkellä ole hyvitystä
- Tämä peruutus vähentää 87,74 $ hyvitysrajasta, joka on 50 000 $.
- Jos vaihdat, uuden ostoksen kokonaisarvon pitäisi olla suurempi kuin 87,74 $.

**Edellisen laskutusjakson laskua ei voi nähdä**

Joitakin mahdollisia syitä, joiden vuoksi et ehkä näe laskua:

- Sinulla on kuukausittaisen saldon määrä tilauksessasi, jonka ylitit tai jonka olet saanut maksuttomasta kokeiluversiosta. Lasku luodaan vain, kun velkasi on
- Azuren tilauspäivä on alle 30 päivän päässä
- Laskua ei ole vielä luotu. Odota laskutusjakson loppuun asti
- Jos et ole tilin järjestelmänvalvoja, vanhemmat laskut eivät ehkä ole käytettävissäsi

**Laskun lataaminen Azure-portaalista (.pdf)**

- Valitse tilauksesi [Azure-portaalin](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Tilaukset-sivulta [käyttäjänä, jolla on pääsy laskuihin](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Valitse **laskut**
- Valitse **Lataa lasku,** jos haluat tarkastella PDF-laskun kopiota. Jos siinä lukee **Ei käytettävissä,** katso miksi [en näe laskua viimeiseksi laskutusjaksoksi?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

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

Muita kysymyksiä: [Tutustu varattuihin esiintymien tiedostoihin](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Suositellut asiakirjat**

- [Laskutuksen perusteet](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Tietoja varatun esiintymän alennuksen alennuksesta](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure-laskutuslaskun ja päivittäisten käyttötietojen lataaminen tai tarkasteleminen](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Tietoja varatun esiintymän alennuksen alennuksesta](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Tietoja Pay-As-You-Go -tilauksesi varatun esiintymän käytöstä](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Enterprise-rekisteröinnin varatun esiintymän käytön ymmärtäminen](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows-ohjelmiston kustannukset, jotka eivät sisälly varattuihin esiintymään](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Varatut esiintymät Partner Central Cloud Solution Provider (CSP) -ohjelmassa](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)