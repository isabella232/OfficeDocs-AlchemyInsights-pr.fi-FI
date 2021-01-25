---
title: Todennusongelmat
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: 53bd0d8f8edaead519d0282239d3a6d338b297b9
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974489"
---
# <a name="authentication-issues"></a>Todennusongelmat

**Etsitkö tietoja Azure Active Directory (Azure AD) -suojaustunnuspalvelusta (STS) palautetuista AADSTS-virhekoodeista?** Katso [Azure AD -todennuksen ja valtuutuksen virhekoodeista](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) AADSTS-virheen kuvaukset, korjaukset ja joitakin ehdotettuja vaihtoehtoisia ratkaisuja.

Valtuutusvirheet voivat johtua useista eri ongelmista, joista useimmat luovat 401- tai 403-virheen. Esimerkiksi seuraavat ongelmat voivat johtaa valtuutusvirheisiin:

- Virheelliset [käyttöoikeustietueen hankintavirrat](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- Huonosti määritetyt [käyttöoikeuksien laajuudet](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- Suostumuksen [puute](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

Jos haluat ratkaista yleisiä valtuutusvirheitä, kokeile alla olevia ohjeita, jotka vastaavat läheisimmin vastaanottamastasi virheestä. Näyttöön saattaa tulla virhe, joka koskee useita vaiheittaista vaihetta.

- **401 Luvaton virhe: Kelpaako tunnus?**

Varmista, että sovelluksesi esittää microsoft Graphin kelvollisen käyttöoikeustietueen osana pyyntöä. Tämä virhe tarkoittaa usein sitä, että käyttöoikeustietue saattaa puuttua HTTP-todennuspyynnön otsikosta tai että tunnus on virheellinen tai vanhentunut. On erittäin suositeltavaa käyttää Microsoftin todennuskirjastoa (MSAL) käyttöoikeustietueiden hankintaan. Lisäksi tämä virhe voi ilmetä, jos yrität käyttää henkilökohtaiselle Microsoft-tilille myönnettyä delegoitua käyttöoikeustietueen avulla ohjelmointirajapintaa, joka tukee vain työ- tai koulutilejä (organisaatiotilit).

**403 Kielletty -virhe: Oletko valinnut oikeat käyttöoikeudet?**

Varmista, että olet pyytänyt oikeat käyttöoikeudet sovelluspuheluiden Microsoft Graph -ohjelmointirajapintojen perusteella. Suositellut järjestelmänvalvojan oikeudet on annettu kaikissa Microsoft Graph -ohjelmointirajapinnan ohjeaiheissa. Lisäksi käyttäjän tai järjestelmänvalvojan on myönnettävä nämä käyttöoikeudet sovellukseen. Käyttöoikeuksien myöntäminen tapahtuu tavallisesti Azure Portal -sovelluksen rekisteröintikoneen suostumuksen sivulla tai käytössä. Valitse **sovelluksen** Asetukset-sovelluksesta **Pakolliset käyttöoikeudet** ja valitse sitten **Myönnä käyttöoikeudet.** Lisätietoja on seuraavissa artikkeleissa:

- [Microsoft Graphin käyttöoikeudet](https://docs.microsoft.com/graph/permissions-reference) 
- [Tietoja Azure AD:n käyttöoikeuksista ja suostumuksesta](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**403 Kielletty -virhe: Hankkiko sovellus tunnuksen, joka vastaa valittuja käyttöoikeuksia?**

Varmista, että pyydetyt tai myönnetyt käyttöoikeustyypit vastaavat sovelluksen hankkimaa käyttöoikeustietuetyyppiä. Saatat pyytää ja myöntää sovelluksen käyttöoikeuksia, mutta käytät delegoituja vuorovaikutteisia koodinkulkutunnuksia asiakkaan tunnistetietojenkulkutunnusten sijaan tai pyydät ja myöntävät delegoituja käyttöoikeuksia, mutta käytät asiakkaan tunnistetietovuotunnuksia valtuutisten kooditunnusten sijaan.

Lisätietoja tunnusten hankkimisesta on kohdassa:

- [Käyttöoikeuden saaminen käyttäjien puolesta ja delegoidut käyttöoikeudet](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v2.0 - OAuth 2.0 -valtuutuskoodin kulku](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Käyttöoikeuden saaminen ilman käyttäjää (daemon-palvelu) ja sovelluksen käyttöoikeuksia](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v2.0 – OAuth 2.0 -asiakasohjelman tunnistetietojen kulku](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**403 Kielletty -virhe: salasanan vaihtaminen**

Tällä hetkellä ei ole sovelluksen käyttöoikeus daemon-palvelun käyttöoikeuksia, jotka sallivat käyttäjien salasanojen vaihtamisen. Näitä ohjelmointirajapintoja tuetaan vain vuorovaikutteisten valtuutetuissa koodivirroissa kirjautuneen järjestelmänvalvojan kanssa. Lisätietoja on kohdassa [Microsoft Graph -käyttöoikeudet.](https://docs.microsoft.com/graph/permissions-reference)

**403 Kielletty: Onko käyttäjällä käyttöoikeus ja onko hänellä käyttöoikeus?**

Microsoft Graph arvioi valtuutetuissa koodivirroissa, onko pyyntö sallittu sovellukseen myönnettyjen käyttöoikeuksien ja kirjautuneen käyttäjän käyttöoikeuksien perusteella. Yleensä tämä virhe tarkoittaa, että käyttäjällä ei ole  tarpeeksi käyttöoikeuksia pyynnön suorittamiseen tai että käyttäjällä ei ole käyttöoikeutta tietoihin, joita hän käyttää. Vain käyttäjät, joilla on tarvittavat käyttöoikeudet, voivat tehdä pyynnön onnistuneesti.

**403 Kielletty: Oletko valinnut oikean resurssirajapinnan?**

Api-palvelut, kuten Microsoft  Graph, tarkistavat, että vastaanottaneen käyttöoikeustietueen oletusarvo (käyttäjäryhmä) vastaa itse odottamaansa arvoa, ja jos näin ei ole, tapahtuu 403 Kielletty-virhe. Yleinen virhe, joka johtaa tähän virheeseen, yrittää käyttää Azure AD Graphin ohjelmointirajapintojen, Outlook-ohjelmointirajapintojen tai SharePointin/OneDriven ohjelmointirajapintojen tunnuksia Microsoft Graphiin kutsumaan (tai päinvastoin). Varmista, että sovellus hankkii resurssin (tai laajuuden), joka vastaa sovelluksen kutsumaa ohjelmointirajapintaa.

**400 Virheellinen pyyntö tai 403 Kielletty: Noudattaako käyttäjä organisaation ehdollisia käyttöoikeuskäytäntöjä?**

Organisaation ehdollisten käyttökäytäntöjen (CA) perusteella käyttäjä, joka käyttää Microsoft Graph -resursseja sovelluksen kautta, saattaa olla haastavaa saada lisätietoja, joita ei ole alun perin hankitussa käyttöoikeustietueessa. Tässä tapauksessa sovelluksesi saa **virheilmoituksen 400 *interaction_required*** tunnuksen hankintaan tai **403-virheeseen, *insufficient_claims*** microsoft Graphia kutsuttaessa. Kummassakin tapauksessa virhevastaus sisältää lisätietoja, jotka voidaan esittää hyväksytylle päätepisteille, jotta käyttäjä voi saada lisätietoja (kuten monimenetelmäisen todentamisen tai laitteen rekisteröinnin).

Lisätietoja ehdollisesta käyttöomme liittyvästä on kohdassa:

- [Ehdollisten access-haasteiden käsittely MSAL:n avulla](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Kehittäjän ohjeet Azure Active Directoryn ehdolliseen käyttöön](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Azure Active Directory -todennuskirjaston (ADAL) ja Azure AD Graph API:n (AAD Graph) tuen päättyminen_* _

- 30. kesäkuuta 2020 alkaen Uusia ominaisuuksia ei enää lisätä Azure Active Directory -todennuskirjastoon (ADAL) ja Azure AD Graph API:een (AAD Graph). Teknisen tuen ja suojauspäivitysten tarjoaminen jatkuu, mutta ominaisuuspäivityksiä ei enää tarjota.
- 30. kesäkuuta 2022 alkaen ADAL: n ja AAD Graphin tuki päättyy, eikä se enää tarjoa teknistä tukea tai suojauspäivityksiä.
    - Sovellukset, jotka käyttävät ADAL:tä nykyisissä käyttöjärjestelmäversioissa, toimivat edelleen tämän ajan kuluttua, mutta eivät saa teknistä tukea tai suojauspäivityksiä.
    - AAD Graphia tämän jälkeen käyttävät sovellukset eivät ehkä enää saa vastauksia AAD Graph -päätepisteltä.

_ *ADAL-siirto**

Suosittelemme päivittämään [Microsoftin todentamiskirjastoon (MSAL),](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)jossa on uusimmat ominaisuudet ja suojauspäivitykset. Tämä suositus koskee sitä, että Microsoft siirretään sovellukset MSAL:lle tuen päättymisajan loppuun mennessä. Microsoft-sovellusten MSAL-siirtoon tavoitteena on varmistaa, että sovellukset hyötyvät MSAL:n jatkuvia suojaus- ja ominaisuusparannuksia.

- [ADAL:n usein kysytyt kysymykset](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Opi siirtämään sovelluksia käyttöympäristökohtaisesti](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Jos tarvitset apua sen ymmärtämiseen, mitkä sovelluksistasi käyttävät ADAL:tä, suosittelemme tarkistamaan kaikki sovellusten lähdekoodit, ja ota tarvittaessa yhteyttä kaikkiin itsenäisten ohjelmistotoimittajien (ISV) tai sovellustoimittajien kanssa. Microsoft-tuki voi myös tarjota sinulle luettelon kaikista vuokraajan ei-Microsoft ADAL -sovelluksista.

**AAD Graph -siirto**

Jos sovellus käyttää AAD Graphia, noudata ohjeita azure AD Graph -sovellusten [siirtämiseksi Microsoft Graphiin.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true)

- [Siirron tarkistusluettelomme tarjoaa aloituspisteen.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist) 
- Azure-sovelluksen rekisteröintiportaali näyttää, mitkä sovellukset käyttävät AAD Graphia. Suosittelemme, että tarkistat kaikki sovellusten lähdekoodit, ja ota tarvittaessa yhteyttä internet-palveluntarjoajiin tai sovelluspalveluntarjoajiin. Microsoft-tuki voi myös antaa sinulle tietoja vuokraajan kaikista AAD Graph -käytöstä.

 










