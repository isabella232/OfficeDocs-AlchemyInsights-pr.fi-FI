---
title: Miksi Lisää budjetti -painike on poissa käytöstä?
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
- "9003547"
- "6464"
ms.openlocfilehash: 426a54ea22490dcc47f40fd990654b2cf051a058
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822632"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Miksi Lisää budjetti -painike on poissa käytöstä?

Budjetin luomiseen tarvitaan jokin seuraavista käyttöoikeuksista:

- Management Group, Subscription, Resource Group Scopes
- Kustannusten hallinnan avustaja
- Omistaja
- Osallistuja
- Vain yritysasiakas: rekisteröinti, osasto, tilin laajuus
- Rekisteröintien järjestelmänvalvoja (määritä budjetti rekisteröintialueen mukaan)
- Osaston järjestelmänvalvoja (määritetty budjetti Osasto-kohdassa)
- Tilin omistaja (määritetty budjetti Tilin laajuus -kohdassa)
- Vain moderni asiakassopimus: Laskutustili, laskutusprofiili, laskuosion laajuus
- Azure-tilauksen luoja

**Loin budjetin, kun kuluvan kuukauden kustannukset olivat jo ylibudjetin. Miksi en saanut ilmoitusta?**  
Jos olet jo ylittänyt tietyn kustannusrajan, kun luot budjetin, jota ilmoitus ei tule. Kun uusi jakso alkaa ja rikot raja-arvon, ilmoitus käynnistyy.

**Milloin voin odottaa saavan ilmoituksen, kun ylitän jonkin määritetyn budjetti-ilmoituksen raja-arvon?**  
Budjetit arvioidaan neljän tunnin välein. Käyttötietojen saavuttaminen budjettijärjestelmään kestää vähintään 8 tuntia. Jos tämä on tehty, ilmoitusten tuleminen voi kestää enintään 12 tuntia, kun raja-arvo ylitit.

**Miksi Aloituspäivä-painike on poissa käytöstä, kun valitsen kuukauden tai laskutuskuukauden palautusjakson?**  
Budjetit tasataan nykyisen kalenterikuukauden tai nykyisen laskutusjakson mukaan (jos Laskutuskuukausi on valittuna). Siksi esitäytämme tämän arvon valmiiksi.

**Miksi en näe kaaviota budjetin luomisen kustannuksista?**  
Tarvitsemme vähintään kaksi kuukautta kustannustietoja, ennen kuin voimme hahmontaa kaavion, joka auttaa budjetin luomisessa.

**Miksi en voi määrittää budjettia juuri luomani tilauksen mukaan?**  
Tilauksen luomisen jälkeen tietojen käsittely kestää 24–48 tuntia, ennen kuin budjetti määritetään siihen.

**Budjetin ohjelmointirajapinnan resurssit**

- [Budjettien ohjelmointirajapinta v1:](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support)Tarjoaa toimintoja budjettien luomiseen ja päivittämiseen. Budjetit-ohjelmointirajapinnan avulla voit määrittää budjetin raja-arvon ja määrittää useita ilmoituksia tulemaan, kun lähestyt raja-arvoa. Ilmoitukset voivat käynnistää sähköpostin tai Azure-toimintoryhmän automaation suorittamiseksi. Huomautus: Tämän ohjelmointirajapinnan suodatus ei vastaa kyselyn ohjelmointirajapinnan suodatusta/dimensioita.
- [Budjettien ohjelmointirajapinta v2:](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json)Luo budjetteja, joissa on suurempia kustannussuodatusominaisuuksia kuin v1. Suodatus tasataan kysely- ja dimensioiden ohjelmointirajapintojen sopimukseen. Tämä on suositeltu budjettien ohjelmointirajapinta, jotta sitä voi käyttää eteenpäin.
- [Dimensiot:](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support)Tarjoaa toimintoja, jotka saavat käyttösi tuetut mitat erilaisilla käyttöalueilla. Dimensions API -ohjelmointirajapinnan avulla voit noutaa dimensioluettelon, jota voidaan käyttää kyselyjen luomisen syötteenä kyselyn ohjelmointirajapinnan avulla.
- [Kysely:](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)Tarjoaa toimintoja, jotka keräät koostettuja kustannus- ja käyttötietoja kyselyn perusteella. Kyselyn ohjelmointirajapinnan avulla voit määrittää haluamasi suodatuksen, lajittelun ja ryhmittelyn kaikkien käytettävissä olevien dimensioiden mukaan (joita käytetään Dimensiot-ohjelmointirajapinnasta).

**Ennustetut kustannukset**

**Miksi kustannusanalyysissa ei ole ennusteita kustannuksista?**  
Ennusteen projektion voi puuttua kustannusanalyysissa useista eri syistä, joista jotkin ovat seuraavat:

1. Jos kustannustiedot ovat alle 10 päivää vanhoja, ennustekaavio ei lataudu. Malli edellyttää vähintään 10 päivää viimeisimpien kustannustietojen tarkan ennusteen varten.
2. Jos olet valinnut historialliset päivämäärät, ennustekaavio ei näy. Valitse päivämääräalue, jossa näkyvät tulevat päivämäärät ennustekaaviolle
3. Jos tililläsi on useita valuuttoja, ennustekaaviossa projektikustannukset tulevat vain "Kaikki kustannukset Yhdysvaltain dollareina" -kohdan osalta.

**Miksi ennuste ei muutu, kun teen muutoksia resursseihini?**  
Ennustemalli vaatii muutaman päivän, jotta tiliin tehdyt muutokset voidaan ottaa huomioon, eikä se tee välittömiä ennusteita resurssien muutosten perusteella  
Resurssien suurentamisen tai pienenemisen vaiheiden vuoksi malliin mukautuminen poikkeamien varalta kestää hieman kauemmin.

**Miksi ennusteeni kasvaa, kun teen varauksen tai Marketplacen oston?**  
Ennustemalli ottaa huomioon Toteutuneet kustannukset -tunnuksesi eikä ota huomioon käyttöä ja ostoa erikseen. Kertaostoksena hankittavissa kustannuksissa ennusteet pienenevät 10 päivän kuluttua.

**Haluan nähdä yhden dimension ennusteet (esimerkiksi Metri)**  
Ennuste tukee tällä hetkellä kokonaiskustannuksia, ei yksittäisiä metrejä. Kun dimensio on Ryhmitelty, ennusteet koskevat dimension kaikkien kohteiden kokonaissummaa.

**Suositellut asiakirjat**

- [Mikä on Azure Cost Management?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azuren kustannustenhallinnan parhaat käytännöt](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kustannusten ja rahan analysoiminen](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kustannusten tutkiminen ja analysoiminen kustannusanalyysin avulla](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure Cost Management: Hinnoittelu](https://azure.microsoft.com/services/cost-management/#pricing)
- [Kustannusten tarkasteleminen kustannusanalyysissa](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Opetusvideo: Budjetin luominen Azure-portaalissa](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Budjetteja tarkastelemisen ja mukauttamisen edellytykset](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Budjettien luominen ja hallinta](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Automaation määrittäminen Azuren toimintoryhmien ja budjettien ohjelmointirajapinnan avulla](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Käytön ja rahankäytön seuranta kustannusilmoituksilla](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kustannusten hallinnan parhaat käytännöt](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Opetusohjelmavideot**

- [Budjetin luominen Azure-portaalissa](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Kustannusten hallinta Budjetin ohjelmointirajapinnan ja toimintoryhmien avulla](https://go.microsoft.com/fwlink/?linkid=2147038)