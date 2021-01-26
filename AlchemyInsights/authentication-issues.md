---
title: Todentaminen
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
ms.openlocfilehash: 2f413e863e6aa23548e425de5901f8158e1d48ab
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/25/2021
ms.locfileid: "49976846"
---
# <a name="authentication-issues"></a>Todentaminen

**Etsitkö tietoja Azure Active Directoryn (Azure AD) suojaustunnuspalvelusta (STS) palautetuista AADSTS-virhekoodeista?** Katso [Azure AD -todennuksen ja valtuutusten virhekoodien](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) AADSTS-virheiden kuvaukset, korjaukset ja joitakin ehdotettuja ratkaisuja.

Valtuutusvirheet voivat johtua useista erilaisista ongelmista, joista useimmat luovat 401- tai 403-virheen. Esimerkiksi seuraavat ongelmat voivat kaikki johtaa valtuutusvirheisiin:

- Virheelliset [tunnusoston työnkulut](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- Huonosti määritetyt [käyttöoikeuksien laajuudet](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- [puuttuminen](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

Voit ratkaista yleisiä valtuutusvirheitä kokeileminen alla olevia ohjeita, jotka vastaavat läheisimmin saamistasi virheistä. Useampi kuin yksi vaihe saattaa päteä saamaasi virheeseen.

**401 Valtuuttamaton virhe: Kelpaako tunnus?**

Varmista, että sovellus esittää kelvollisen Microsoft Graph -käyttöoikeustietueen pyynnön osana. Tämä virhe tarkoittaa usein, että käyttöoikeustietue saattaa puuttua HTTP-todennuspyynnön otsikosta tai että tunnus on virheellinen tai vanhentunut. Microsoft suosittelee voimakkaasti, että käytät Microsoftin todennuskirjastoa (MSAL) käyttöoikeustietueiden hankkimiseen. Lisäksi tämä virhe voi ilmetä, jos yrität käyttää henkilökohtaiselle Microsoft-tilille myönnettyä valtuullista käyttöoikeustietuetta ja käytät ohjelmointirajapintaa, joka tukee vain työ- tai koulutilejä (organisaatiotilit).

**403 Kielletty virhe: Oletko valinnut oikeat käyttöoikeudet?**

Varmista, että olet pyytänyt oikeaa käyttöoikeusjoukkoa sovelluspuheluiden Microsoft Graph -ohjelmointirajapintojen perusteella. Suositellut järjestelmänvalvojan oikeudet ovat käytettävissä kaikissa Microsoft Graph API -ohjelmointirajapinnan ohjeaiheissa. Lisäksi käyttäjän tai järjestelmänvalvojan on myönnettävä käyttöoikeudet sovellukseen. Käyttöoikeuksien myöntäminen tapahtuu yleensä Azure Portal -sovelluksen rekisteröintiä koskevan luvan sivun kautta tai käytön kautta. Valitse **asetukset** valitse sovelluksen **pakolliset käyttöoikeudet** ja valitse sitten **Myönnä käyttöoikeudet**. Lisätietoja on seuraavissa artikkeleissa:

- [Microsoft Graphin käyttöoikeudet](https://docs.microsoft.com/graph/permissions-reference) 
- [Tietoja Azure AD:n käyttöoikeuksista ja hyväksynnästä](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**403 Kielletty virhe: Hankitko sovelluksesta tunnuksen, joka vastaa valittuja käyttöoikeuksia?**

Varmista, että pyydetyt tai myönnetty käyttöoikeustyypit vastaavat sovelluksen hankkimia käyttöoikeustietueita. Saatat pyytää ja myöntää sovelluksen käyttöoikeuksia, mutta käytät valtuutetun vuorovaikutteisen koodinkulkutunnuksia asiakkaan tunnistetietojen työnkulun tunnusten sijaan tai pyydät ja myöntämään valtuutettuja käyttöoikeuksia, mutta käytät asiakastunnusten työnkulun tunnuksia valtuutetun koodinkulkutunnusten sijaan.

Lisätietoja tunnusten hankkimisesta on kohdassa:

- [Käyttöoikeuden saaminen käyttäjien puolesta ja delegoidut käyttöoikeudet](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v2.0 – OAuth 2.0:n valtuutuskoodin kulku](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Käyttöoikeuden saaminen ilman käyttäjää (daemon-palvelu) ja sovelluksen käyttöoikeuksia](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v2.0 – OAuth 2.0 -asiakastietojen kulku](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**403 Kielletty virhe: Salasanan vaihtaminen**

Tällä hetkellä ei ole sovellusten käyttöoikeus daemonin palvelussa käyttöoikeuksia, jotka sallivat käyttäjien salasanojen vaihtamisen. Näitä ohjelmointirajapintoja tuetaan vain vuorovaikutteisten valtuutettujen koodivirtojen avulla kirjautuneen järjestelmänvalvojan kanssa. Lisätietoja on artikkelissa [Microsoft Graphin käyttöoikeudet](https://docs.microsoft.com/graph/permissions-reference).

**403 Kielletty: Onko käyttäjällä käyttöoikeus ja onko hänellä käyttöoikeus?**

Microsoft Graph arvioi valtuutetuissa koodivirroissa, onko pyyntö sallittu sovellukseen myönnettyjen käyttöoikeuksien ja sisään kirjautuneen käyttäjän käyttöoikeuksien perusteella. Yleensä tämä virhe tarkoittaa, että käyttäjällä ei ole järjestelmänoikeutta tehdä pyyntöä **eikä** käyttäjällä ei ole käyttöoikeutta tietoihin, joita hän voi käyttää. Vain käyttäjät, joilla on tarvittavat käyttöoikeudet, voivat tehdä pyynnön onnistuneesti.

**403 Kielletty: Oletko valinnut oikean resurssien ohjelmointirajapinnan?**

Ohjelmointirajapintapalvelut, kuten Microsoft Graph, tarkistavat, että *erityisesti* lunastaa (yleisön) vastaanottaneen käyttöoikeustietueen arvon, ja jos näin ei ole, tapahtuu 403 kielletty virhe. Yleinen virhe, joka aiheuttaa tämän virheen, yrittää käyttää Azure AD Graph -ohjelmointirajapintojen, Outlook-ohjelmointirajapintojen tai SharePoint- tai OneDrive-ohjelmointirajapintojen hankkimaa tunnusta Microsoft Graphin kutsumisen (tai päinvastoin). Varmista, että sovellus hankkii resurssin (tai laajuuden), joka vastaa sovelluksen kutsumaa ohjelmointirajapintaa.

**400 Virheellinen pyyntö tai 403 Kielletty: Noudattaako käyttäjä organisaation ehdollisia käyttöoikeuskäytäntöjä?**

Organisaation ehdollisten käyttöoikeuskäytäntöjen (CA) mukaan käyttäjä, joka käyttää Microsoft Graph -resursseja sovelluksen kautta, voi olla haastavaa saada lisätietoja, joita ei ole sovelluksen alun perin hankkimassa käyttöoikeustietueessa. Tässä tapauksessa sovellus saa **400 -virheen *interaction_required*** access-tunnusoston tai **403:n *insufficient_claims*** Microsoft Graphia kutsuttaessa. Kummassakin tapauksessa virhevastaus sisältää lisätietoja, jotka voidaan esittää valtuutettuun päätepisteeseen, jotta käyttäjä voi saada lisätietoja (esimerkiksi monimenetelmäisen todentamisen tai laiterekisteröimisen).

Lisätietoja ehdollisesta käyttöoikeudesta löydät kohteesta:

- [Ehdollisten käytön haasteiden käsitteleminen MSAL:lla](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Azure Active Directoryn ehdollisen käytön opas kehittäjälle](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide) käyttö

**_Azure Active Directory -todentamiskirjaston (ADAL) ja Azure AD Graph API:n (AAD Graph) tuen päättyminen_* _

- 30. kesäkuuta 2020 alkaen Microsoft ei enää lisää uusia ominaisuuksia Azure Active Directory -todentamiskirjastoon (ADAL) ja Azure AD Graph API:iin (AAD Graph). Tarjoamme jatkossakin teknistä tukea ja suojauspäivityksiä, mutta emme enää tarjoa ominaisuuspäivityksiä.
- 30. kesäkuuta 2022 alkaen Microsoft lopettaa ADAL- ja AAD Graph -tuen, eikä Microsoft enää tarjoa teknistä tukea tai suojauspäivityksiä.
    - Sovellukset, jotka käyttävät ADAL:tä olemassa olevissa käyttöjärjestelmäversioissa, toimivat edelleen tämän ajan kuluttua, mutta eivät saa teknistä tukea tai suojauspäivityksiä.
    - AAD Graphia tämän jälkeen käyttävät sovellukset eivät ehkä enää saa vastauksia AAD Graph -päätepisteeltä.

_ *ADAL-siirto**

Suosittelemme päivittämistä [Microsoft todentamiskirjastoon (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), jossa on uusimmat ominaisuudet ja suojauspäivitykset. Tämä suositus johtuu sitä, että Microsoft on siirtää sovellukset MSAL:ään tuen päättymispäivään mennessä. Microsoft-sovellusten MSAL:ään siirtymisen tavoitteena on varmistaa, että sovellukset hyötyvät MSAL:n jatkuvista suojaus- ja ominaisuusparannuksista.

- [Lue ADAL:ää koskevat usein kysytyt kysymykset](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Lisätietoja sovellusten siirtämisestä käyttöympäristökohtaisesti](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Jos tarvitset apua siitä, mikä sovelluksistasi käyttää ADAL:ää, on suositeltavaa tarkistaa kaikkien sovellusten lähdekoodi ja ottaa tarvittaessa yhteyttä riippumattomaan ohjelmistotoimitsijaan (ISV)- tai sovellustoimitsijaan. Microsoftin tukipalvelu voi myös tarjota sinulle luettelon kaikista vuokraajan ei-Microsoft ADAL -sovelluksista.

**AAD Graph -siirto**

AAD Graphia käyttävissä sovelluksissa, noudata opasta [Azure AD Graph -sovellusten siirtäminen Microsoft Graphiin](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Siirron tarkistusluettelo tarjoaa aloituspisteen](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- Azure-sovelluksen rekisteröintiportaali näyttää, mitkä sovellukset käyttävät AAD Graphia. Suosittelemme, että tarkistat kaikki sovellusten lähdekoodit. Ota tarvittaessa yhteyttä internet-palveluntarjoajaan tai sovelluksen toimittajaan. Microsoftin tuki voi myös antaa tietoja kaikesta AAD Graphin käytöstä vuokraajallasi.

 










