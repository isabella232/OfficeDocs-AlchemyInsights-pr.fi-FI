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
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974418"
---
# <a name="querying-the-microsoft-graph-api"></a>Microsoft Graph -ohjelmointirajapinnan kysely

Tämä ohjeaihe voi koskea myös kehittäjiä, jotka käyttävät edelleen Azure AD Graph -ohjelmointirajapintaa. On kuitenkin erittäin **suositeltavaa, että** käytät Microsoft Graphia kaikissa hakemisto-, käyttäjätiedot- ja käytönhallintaskenaarioissa.

**Todennus- tai valtuutusongelmat**

- Jos sovellus  ei voi hankkia tunnuksia Microsoft Graph -kutsumista varten, valitse Ongelma, kun saat käyttöoikeustietueen **(todennuksen)** Microsoft Graph -luokan, niin saat tarkempia ohjeita ja tukea tästä aiheesta.
- Jos sovellus saa **401-** tai 403-valtuutusvirheitä Microsoft Graphia kutsuttaessa, valitse Hae käyttö estetty **-virhe (Valtuutus)** Microsoft Graph API -luokka, niin saat tarkempia ohjeita ja tukea tästä aiheesta.

**Haluan käyttää Microsoft Graphia, mutta en tiedä, mistä aloittaa**

Lisätietoja Microsoft Graphista on kohdassa:

- [Yleistä Microsoft Graphista](https://docs.microsoft.com/graph/overview)
- [Yleistä Käyttäjätietojen ja käytön hallinnasta Microsoft Graphissa](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Microsoft Graph -sovellusten rakentamisen aloittaminen](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – Microsoft Graph -ohjelmointirajapintojen testaaminen vuokraajassa tai esittely vuokraajassa

**Haluan käyttää Microsoft Graphia, mutta tukeeko se tarvitsen v1.0-hakemiston ohjelmointirajapinnat?**

Microsoft Graph on hakemiston, käyttäjätietojen ja käytön hallinnan suositeltu ohjelmointirajapinta. Azure AD Graphin ja Microsoft Graphin välillä on kuitenkin vielä muutamia aukkoja. Tutustu seuraaviin artikkeleihin, joissa korostetaan uusimpia eroja, jotka auttavat valitsemaan:

- [Resurssityyppierot Azure AD Graphin ja Microsoft Graphin välillä](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Azure AD Graphin ja Microsoft Graphin ominaisuuden erot](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Azure AD:n ja Microsoft Graphin väliset menetelmäerot](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Kun kyselen *käyttäjäobjektia,* monet sen ominaisuuksista puuttuvat**

`GET https://graph.microsoft.com/v1.0/users` palauttaa vain 11 kohdetta, sillä Microsoft Graph valitsee automaattisesti oletusarvoisen *palautettavan käyttäjäominaisuuksien* joukon. Jos tarvitset muita *käyttäjäominaisuuksia,* $select valita sovelluksen ominaisuudet. Kokeile sitä ensin **Microsoft Graph Explorerissa.**

**Jotkin käyttäjän ominaisuusarvot ovat *tyhjiä,* vaikka tiedän, että ne on määritetty**

Todennäköisin selitys on se, että sovellukselle oli myönnetty *User.ReadBasic.All-käyttöoikeus.* Näin sovellus voi lukea rajoitetun käyttäjäominaisuuksien joukon ja palauttaa kaikki muut ominaisuudet tyhjäarvoksi, vaikka ne olisi aiemmin määritetty. Kokeile myöntää sovelluksen *User.Read.All-käyttöoikeus* sen sijaan.

Lisätietoja on kohdassa [Microsoft Graphin käyttöoikeudet.](https://docs.microsoft.com/graph/permissions-reference#user-permissions)

**I'm having trouble using OData query parameters to filter data in my requests**

Microsoft Graph tukee laajaa valikoimaa OData-kyselyn parametreja, mutta Microsoft Graphin hakemistopalvelut (hakemisto-objektista periytyvät *resurssit)* eivät tue kaikkia näitä parametreja. Samat rajoitukset, joita Azure AD Graphissa oli, säilyvät suurin piirtin Microsoft Graphissa:

1. **Ei tueta:**$count, $search tyhjäarvot ja $filter  *tyhjäarvot*
2. **Ei tueta:**$filter ominaisuuksista (katso resurssiaiheet, joista ominaisuudet ovat suodatettavissa)
3. **Ei tuettu:** sivutus, suodatus ja lajittelu samanaikaisesti
4. **Ei tuettu:** yhteyden suodattaminen. Voit esimerkiksi etsiä kaikki Yhdistyneessä kuningaskunnassa sijaitsevat tekniset ryhmän jäsenet.
5. **Osittainen tuki:**$orderby *(vain* displayName ja userPrincipalName) ja *ryhmä*
6. **Osittainen tuki:** $filter (tukee vain *eq-,* *startswith-* tai ja , ja rajoitettuja) tuki-, $expand (yksittäisen objektin suhteiden laajentaminen palauttaa kaikki yhteydet, mutta objektien suhteiden laajentaminen on rajoitettua)  

Lisätietoja on kohdassa Vastausten [mukauttaminen kyselyparametrien avulla.](https://docs.microsoft.com/graph/query-parameters)

**Ohjelmointirajapinta, johon soitan, ei toimi – missä voin tehdä enemmän testausta?**

**Microsoft Graph Explorer** – Testaa Microsoft Graph -ohjelmointirajapinnat vuokraajassa  tai esittely vuokraajassa ja tutustu myös mallikyselyihin Microsoft Graph Explorerissa.

**Kun kyselen tietoja, näyttää siltä, että saan puutteelliset tiedot takaisin**

Jos kyselet kokoelmaa (kuten *käyttäjiä),* Microsoft Graph käyttää palvelinpuolen sivurajoituksia, joten tulokset palautetaan aina oletussivun kokoisena. Sovelluksen pitäisi aina odottaa näkevän palvelun palauttamia kokoelmia.

Lisätietoja on seuraavissa artikkeleissa:

- [Microsoft Graphin parhaat käytännöt](https://docs.microsoft.com/graph/best-practices-concept)
- [Microsoft Graph -tietojen sivutus sovelluksessa](https://docs.microsoft.com/graph/paging)

**Sovellukseni on liian hidas ja sitä myös käytetään kursivassa. Mitä parannuksia voin tehdä?**

Skenaariostasi riippuen käytettävissäsi on useita vaihtoehtoja, joilla voit tehdä sovelluksesta entistä tehokkaammin ja joissakin tapauksissa vähemmän altis palvelun utelle (kun puheluita on liikaa).

Lisätietoja on ohjeaiheissa:

- [Microsoft Graphin parhaat käytännöt](https://docs.microsoft.com/graph/best-practices-concept)
- [Siirtopyynnöt](https://docs.microsoft.com/graph/json-batching)
- [Muutosten jäljitäminen deltakyselyn avulla](https://docs.microsoft.com/graph/delta-query-overview)
- [Saa ilmoituksia muutoksista verkko-osien kautta](https://docs.microsoft.com/graph/webhooks)
- [Kursimisohjeet](https://docs.microsoft.com/graph/throttling)

**Mistä löydän lisätietoja virheistä ja tunnetuista ongelmista?**

- [Microsoft Graphin virhevastaustiedot](https://docs.microsoft.com/graph/errors)
- [Microsoft Graphin tunnetut ongelmat](https://docs.microsoft.com/graph/known-issues)

**Mistä voin tarkistaa palvelun käytettävyyden ja yhteyden tilan?**

Niiden taustalla olevien palvelujen käytettävyys ja yhteydet, joita voidaan käyttää Microsoft Graphin kautta, voivat vaikuttaa Microsoft Graphin yleiseen käytettävuuteen ja suorituskykyyn.

- Tarkista Azure Active Directory -palvelun kuntoa varten Azure-tilasivulla lueteltujen **suojaus-** ja [käyttäjätietopalvelujen tila.](https://azure.microsoft.com/status/)
- Tarkista Microsoft Graphiin osallistuneet Office-palvelut Office Service Health -koontinäytössä lueteltujen [palvelujen tila.](https://portal.office.com/adminportal/home#/servicehealth)
