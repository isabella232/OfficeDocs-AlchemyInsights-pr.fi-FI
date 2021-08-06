---
title: Microsoft Graph -ohjelmointirajapinnan kysely
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "7846"
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923236"
---
# <a name="querying-the-microsoft-graph-api"></a>Microsoft Graph -ohjelmointirajapinnan kysely

Tämä ohjeaihe voi koskea myös kehittäjiä, jotka käyttävät edelleen Azure AD:Graph ohjelmointirajapintaa. On kuitenkin erittäin suositeltavaa **käyttää** Microsoft Graph kaikissa hakemisto-, käyttäjätiedot- ja käytönhallintaskenaarioissa.

**Todennus- tai valtuutusongelmat**

- Jos sovellus  ei voi hankkia tunnuksia Microsoft Graph-puheluita varten, valitse Ongelma käyttöoikeustunnuksen **(todennuksen)** Microsoft Graph -luokassa, niin saat tarkempia ohjeita ja tukea tästä aiheesta.
- Jos sovellus saa **401-** tai 403-valtuutusvirheitä Microsoft Graph-puheluissa, valitse Käyttö estetty -virhe **(Valtuutus)** Microsoft Graph API -luokka, niin saat tarkempia ohjeita ja tukea tästä aiheesta.

**Haluan käyttää Microsoft Graph, mutta en tiedä, mistä aloittaa**

Lisätietoja Microsoft Graph:

- [Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Yleistä Microsoft Graph:n käyttäjätietojen ja käytön hallinnasta](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Microsoft Graph -sovellusten rakentamisen aloittaminen](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – Microsoft Graph ohjelmointirajapintojen testaaminen vuokraajassa tai esittelytilaajassa

**Haluan käyttää Microsoft Graph, mutta tukeeko se tarvitsen v1.0-hakemiston ohjelmointirajapinnat?**

Microsoft Graph on suositeltu ohjelmointirajapinta hakemiston, käyttäjätietojen ja käytön hallintaan. Azure AD Graph:n ja Microsoft Graph:n mahdollisuuksien välillä on kuitenkin muutamia Graph. Tutustu seuraaviin artikkeleihin, joissa korostetaan ajan tasalla olevaa eroavaisuuksia, jotka auttavat valinnassasi:

- [Azure AD Graph:n ja Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Azure AD -ominaisuuden Graph Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Azure AD:n ja Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Kun kyselen *käyttäjäobjektia,* monet sen ominaisuuksista puuttuvat**

`GET https://graph.microsoft.com/v1.0/users`palauttaa vain 11 kohdetta, Graph Microsoft valitsee automaattisesti palautettavan *käyttäjäominaisuuksien* oletusjoukon. Jos tarvitset muita *käyttäjäominaisuuksia,* $select sovelluksen tarpeita. Kokeile sitä ensin **Microsoft Graph Resurssienhallinnassa.**

**Jotkin käyttäjän ominaisuusarvot ovat *tyhjiä,* vaikka tiedän, että ne on määritetty**

Todennäköisin selitys on se, että sovellukselle on myönnetty *User.ReadBasic.All-käyttöoikeus.* Tällöin sovellus voi lukea rajoitetun käyttäjäominaisuuksien joukon ja palauttaa kaikki muut ominaisuudet tyhjäarvoksi, vaikka ne olisi aiemmin määritetty. Kokeile sovelluksen myöntämistä *sen sijaan User.Read.All-käyttöoikeuden* sijaan.

Lisätietoja on kohdassa [Microsoft Graph käyttöoikeudet.](https://docs.microsoft.com/graph/permissions-reference#user-permissions)

**Minulla on ongelmia OData-kyselyparametrien käyttämisessä pyyntöjen tietojen suodattamiseen**

Microsoft Graph tukee laajaa valikoimaa OData-kyselyparametreja, mutta Microsoft Graph:n hakemistopalvelut (hakemisto-objektista *periytyvät* resurssit) eivät tue kaikkia Graph. Samat rajoitukset, jotka olivat Azure AD Graph säilyvät suurin osa Microsoft Graph:

1. **Ei tueta:**$count-, $search- ja $filter  null-arvoissa *tai ei-tyhjissä* arvoissa
2. **Ei tuettu:**$filter ominaisuuksista (katso resurssiaiheet, joiden ominaisuudet ovat suodatettavissa)
3. **Ei tuettu:** sivutus, suodatus ja lajittelu samanaikaisesti
4. **Ei tuettu:** yhteyden suodattaminen. Etsi esimerkiksi kaikki Yhdistyneessä kuningaskunnassa sijaitsevat tekniset ryhmän jäsenet.
5. **Osittainen tuki:**$orderby *(vain* displayName ja userPrincipalName) ja *ryhmä*
6. **Osittainen tuki:**$filter (tukee vain eq-, *startswith-* tai *,* ja *,* ja rajoitettuja *)*-tukea, $expand (yksittäisen objektin yhteyksien laajentaminen palauttaa kaikki yhteydet, mutta objektien suhteiden laajentaminen on rajoitettua)

Lisätietoja on kohdassa Vastausten [mukauttaminen kyselyparametrien avulla.](https://docs.microsoft.com/graph/query-parameters)

**Ohjelmointirajapinta, johon soitan, ei toimi – missä voin tehdä enemmän testausta?**

**Microsoft Graph Explorer** – Testaa Microsoft Graph -ohjelmointirajapinnat vuokraajassa tai esittelytilaajassa  ja tutustu myös esimerkkikyselyihin Microsoft Graph Resurssienhallinnassa.

**Kun kyselen tietoja, näyttää siltä, että saan taas puutteelliset tiedot**

Jos kyselet kokoelmaa (kuten *käyttäjiä),* Microsoft Graph käyttää palvelinpuolen sivurajoituksia, joten tulokset palautetaan aina oletussivukoon mukaisesti. Sovelluksen pitäisi aina odottaa näkevän palvelun palauttamia kokoelmia.

Lisätietoja on seuraavissa artikkeleissa:

- [Microsoft Graph parhaat käytännöt](https://docs.microsoft.com/graph/best-practices-concept)
- [Microsoftin Graph tietojen sivutus sovelluksessa](https://docs.microsoft.com/graph/paging)

**Sovellukseni on liian hidas ja sitä myös niitetaan. Mitä parannuksia voin tehdä?**

Skenaariostasi riippuen käytettävissäsi on useita vaihtoehtoja, jotka tekevät sovelluksesta entistä tehokkaammin ja joissakin tapauksissa vähemmän altis palvelulle (jos puheluita on liikaa).

Lisätietoja on ohjeaiheissa:

- [Microsoft Graph parhaat käytännöt](https://docs.microsoft.com/graph/best-practices-concept)
- [Siirtopyynnöt](https://docs.microsoft.com/graph/json-batching)
- [Muutosten jäljitäminen deltakyselyn avulla](https://docs.microsoft.com/graph/delta-query-overview)
- [Muutoksista ilmoittaminen webhooksien kautta](https://docs.microsoft.com/graph/webhooks)
- [Throttling guidance](https://docs.microsoft.com/graph/throttling)

**Mistä löydän lisätietoja virheistä ja tunnetuista ongelmista?**

- [Microsoft Graph virhevastaustiedot](https://docs.microsoft.com/graph/errors)
- [Microsoft Graph:n tunnetut ongelmat](https://docs.microsoft.com/graph/known-issues)

**Mistä voin tarkistaa palvelun käytettävyyden ja yhteyden tilan?**

Niiden taustalla olevien palvelujen käytettävyys ja yhteydet, joita voidaan käyttää Microsoft Graph voivat vaikuttaa Microsoft Graph.

- Jos Azure Active Directory palvelun kunto, tarkista Azure-tilasivulla lueteltujen suojaus- ja käyttäjätietopalvelujen [tila.](https://azure.microsoft.com/status/) 
- Jos Office Microsoft Graph-palvelua, tarkista palvelujen tila, joka on lueteltu Office palvelun kunto [-koontinäytössä.](https://portal.office.com/adminportal/home#/servicehealth)
