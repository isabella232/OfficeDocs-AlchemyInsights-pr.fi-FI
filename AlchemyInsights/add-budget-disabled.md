---
title: Miksi lisää budjetti-painike ei ole käytössä?
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
- "9003547"
- "6464"
ms.openlocfilehash: 18edad73f617ba180cb08576ee6e5fa8faf07128
ms.sourcegitcommit: 9a7b85eae0bb775bc2498a83d8f5fedb72a6451e
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807407"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Miksi lisää budjetti-painike ei ole käytössä?

Jos haluat luoda budjetin, sinulla on oltava jokin seuraavista käyttö oikeuksista:

- Hallinta ryhmä, tilaus, resurssi ryhmän alueet
- Kustannusten hallinnan avustaja
- Omistaja
- Avustaja
- Vain Enterprise-asiakas: rekisteröinti, osasto, tili alueet
- Rekisteröinnin järjestelmänvalvoja (budjetin asettaminen rekisteröinnin vaikutus alueella)
- Osaston järjestelmänvalvoja (budjetin asettaminen osaston laajuus)
- Tilin omistaja (budjetin asettaminen tili alueeseen)
- Vain nykyaikainen asiakas sopimus: laskutus tili, laskutus profiili, laskun osaalueet
- Azure-tila uksen luoja

**Loin budjetin, kun kuluvan kuukauden kustannukset olivat jo yli budjetin. Miksi en saa ilmoitusta?**  
Jos olet jo ylittänyt tietyn kustannus kynnyksen, kun luot budjetin, ilmoitus ei syty. Kun uusi sykli alkaa, varoitus tulee näkyviin, jos rikot kynnys arvoa.

**Milloin minun pitäisi odottaa saavansa ilmoituksen, kun ylitän jonkin määritetyn budjetin varoitus kynnysten?**  
Budjetit lasketaan neljän tunnin välein. Se kestää vähintään 8 tuntia, ennen kuin käyttö tiedot saapuvat budjetti järjestelmään. Tämän vuoksi ilmoitusten määrä voi kestää jopa 12 tuntia, kun kynnys arvo ylittyy.

**Miksi aloitus päivä-painike ei ole käytettävissä, kun valitsen kuukauden tai laskutus kuukauden, nollaa kauden?**  
Budjetit tasataan nykyisen kalenteri kuukauden tai nykyisen laskutus kauden mukaan (siinä tapa uksessa, että laskutus kuukausi on valittuna). Siksi tämä arvo on valmiiksi täytetty puolestasi.

**Miksi en näe kustannus kaaviota budjetin luonti kokemuksessani?**  
Tarvitsemme vähintään 2 kuukauden kustannus tietoja, ennen kuin voimme tehdä kaaviosta apua budjetin luomisessa.

**Miksi en pysty määrittämään budjettia juuri luomaasi tila ukseen?**  
Kun tilaus on luotu, tietojen käsittely kestää 24-48 tuntia ennen budjetin määrittämistä.

**Budjetin API-resurssit**

- [Budjetit-ohjelmointi raja pinta v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): Luo ja Päivitä budjetteja. Budjetit-ohjelmointi raja pinnan avulla voit määrittää budjetin kynnys arvon ja määrittää useita hälytyksiä tuleen, kun lähestyt tätä kynnys arvoa. Ilmoitukset voivat käynnistää sähkö postin tai Azure-toiminto ryhmän automaation suorittamista varten. Huomautus: tämän API-liittymän suodattaminen ei Tasaa kyselyn API-suodatukseen/-dimensioihin.
- [Budjetit-ohjelmointi raja pinta v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): Luo budjetteja, joilla on suuremmat kustannukset suodatus ominaisuudet kuin v1. Suodatus tasataan kysely-ja dimensiot-ohjelmointi raja pintojen käyttämään sopimukseen. Tämä on suositellut budjetit-ohjelmointi raja pinta, jonka avulla siirrytään eteenpäin.
- [Mitat](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): sisältää toimintoja, joiden avulla saat käyttöön tuettavat dimensiot eri käyttö alueissa. Dimensiot-ohjelmointi raja pinnan avulla voit noutaa luettelon dimensioista, joita voi käyttää kyselyjen luomisessa kyselyn ohjelmointi raja pinnan avulla.
- [Kysely](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): sisältää toimintoja, joiden avulla saat koostetut kustannukset ja käyttö tiedot toimittamiesi kyselyjen perusteella. Kysely-ohjelmointi raja pinnan avulla voit määrittää haluamasi suodatuksen, lajittelun ja ryhmittelyn kaikkiin käytettävissä oleviin dimensioihin (joita käytetään dimensioista ohjelmointi raja pinnasta).

**Ennustetut kustannukset**

**Miksi kustannus analyysin kustannukset eivät näy?**  
On useita syitä siihen, miksi ennusteen projektio saattaa puuttua sinulle kustannus analyyseissä, joista osa on seuraavanlaisia:

1. Jos hinta tiedot ovat alle 10 päivää vanhoja, ennuste kaaviota ei ladata. Malli vaatii vähintään 10 päivää uusimpien hinta tietojen tarkat ennusteet
2. Jos olet valinnut historialliset päivä määrät, ennuste kaavio ei ole näkyvissä. Valitse päivämäärä väli, jossa ennuste kaavion tulevat päivä määrät näytetään
3. Jos tililläsi on useita valuuttoja, ennuste kaavio sisältää vain kustannukset, jotka aiheutuvat kaikista kustannuksista dollareissa.

**Miksi ennuste ei muutu, kun teen muutoksia omiin resursseihin?**  
Ennuste malli edellyttää parin päivän tilin muuttamista, eikä se tee välittömiä ennusteita resurssi muutosten perusteella.  
Jos haluat suurentaa tai pienentää resursseja entistä enemmän, malli kestää hieman kauemmin, jotta muutokset mukautuvat näihin muutoksiin.

**Miksi ennuste kasvaa, kun teen vara uksen tai Marketplace-ostoksen?**  
Ennuste malli ottaa huomioon todelliset kustannukset, eikä sitä voi ottaa käyttöön ja ostaa erikseen. Kerta ostoksena, malli laskee ennusteet 10 päivän kuluttua, jotta kustannukset kasvavat äkillisesti.

**Haluan nähdä yksittäisen dimension ennusteet (esim. Mittari**  
Ennuste tukee tällä hetkellä kokonaiskustannusennusteita eikä yksittäisiä mittareita. Näin ollen kun on ryhmitelty dimensiolla, ennusteet ovat kaikkien dimension kohteiden summa.

**Suositellut asia kirjat**

- [Mikä on Azure Cost Management?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure Cost Managementin parhaat käytännöt](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kustannusten ja kulujen analysointi](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kustannus analyysin kustannusten tutkiminen ja analysoiminen](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure Cost Management: hinnoittelu](https://azure.microsoft.com/services/cost-management/#pricing)
- [Kustannus analyysin kustannusten tarkasteleminen](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Video-opetus ohjelma: budjetin luominen Azure-portaalissa](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Budjettien tarkastelun ja mukauttamisen edellytykset](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Budjettien luominen ja hallinta](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Automatisoinnin määrittäminen Azure-toiminta ryhmien ja budjettien ohjelmointi raja pinnan avulla](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Käytön ja kulutuksen valvonta kustannusten ilmoitusten avulla](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kustannusten hallinnan parhaat käytännöt](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Opetus videot**

- [Budjetin luominen Azure-portaalissa](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Kustannusten hallinta budjettien ohjelmointi raja pinnan ja toiminta ryhmien avulla](https://go.microsoft.com/fwlink/?linkid=2147038)