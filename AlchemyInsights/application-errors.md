---
title: Sovellusvirheet
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "7841"
ms.openlocfilehash: ce4c89da79112726ed4fb25527edc8d082bd37f239595b9eab7279abeeecfd7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931446"
---
# <a name="application-errors"></a>Sovellusvirheet

Etsitkö tietoja **AADSTS-virhekoodeista,** jotka palautetaan Azure Active Directory (Azure AD) -suojaustunnuspalvelusta (STS)? Lue [Azure AD -todennuksen ja valtuutusvirhekoodien](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) avulla AADSTS-virheiden kuvaukset, korjaukset ja joitakin ehdotettuja vaihtoehtoisia ratkaisuja.

Valtuutusvirheet voivat johtua useista erilaisista ongelmista, joista useimmat luovat 401- tai 403-virheen. Esimerkiksi seuraavat voivat johtaa valtuutusvirheisiin:

- Virheelliset [tunnusoston työnkulut](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- Huonosti määritetyt [käyttöoikeuksien laajuudet](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- [puuttuminen](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Voit ratkaista yleisiä valtuutusvirheitä noudattamalla alla olevia ohjeita, jotka vastaavat läheisimmin vastaanottamiasi virheitä. Useita voi olla.

**401 Valtuuttamaton virhe: Kelpaako tunnus?**

Varmista, että sovelluksesi esittää Microsoft Graph kelvollinen käyttöoikeustietue pyynnön osana. Tämä virhe tarkoittaa usein, että käyttöoikeustietue saattaa puuttua HTTP-todennuspyynnön otsikosta tai että tunnus on virheellinen tai vanhentunut. On erittäin suositeltavaa käyttää [Microsoftin todentamiskirjastoa (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) käyttöoikeustietueiden hankkimiseen. Lisäksi tämä virhe voi ilmetä, jos yrität käyttää henkilökohtaiselle Microsoft-tilille myönnettyä delegoitua käyttöoikeustietueen avulla ohjelmointirajapintaa, joka tukee vain työ- tai koulutilejä (organisaatiotilit).

**403 Kielletty virhe: Oletko valinnut oikeat käyttöoikeudet?**

Tarkista, että olet pyytänyt oikeita käyttöoikeuksia sovelluspuheluiden Microsoft Graph ohjelmointirajapintojen perusteella. Suositeltuja käyttöoikeuksia on saatavilla kaikissa Microsoft Graph -ohjelmointirajapinnan ohjeaiheissa. Lisäksi käyttäjän tai järjestelmänvalvojan on myönnettävä käyttöoikeudet sovellukseen. Käyttöoikeuksien myöntäminen tapahtuu yleensä suostumussivun kautta tai myöntämällä käyttöoikeuksia Azure Portal -sovelluksen rekisteröintiterällä. Valitse **asetukset** valitse sovelluksen **pakolliset käyttöoikeudet** ja valitse sitten **Myönnä käyttöoikeudet**.

- [Microsoft Graphin käyttöoikeudet](https://docs.microsoft.com/graph/permissions-reference) 
- [Tietoja Azure AD:n käyttöoikeuksista ja hyväksynnästä](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 Kielletty virhe: Hankitko sovelluksesta tunnuksen, joka vastaa valittuja käyttöoikeuksia?**

Varmista, että pyydettyjen tai myönnettyjen käyttöoikeuksien tyyppi vastaa sovelluksen hankkimaa käyttöoikeustietuetyyppiä. Saatat pyytää ja myöntää sovelluksen käyttöoikeuksia, mutta käytät delegoituja vuorovaikutteisia kooditunnuksia asiakkaan tunnistetietovuotunnusten sijaan tai pyydät ja myöntämään delegoidut käyttöoikeudet, mutta käytät asiakkaan tunnistetietovuotunnuksia delegoidun koodin kulkutunnusten sijaan.

- [Käyttöoikeuden saaminen käyttäjien puolesta ja delegoidut käyttöoikeudet](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v2.0 – OAuth 2.0:n valtuutuskoodin kulku](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Käyttöoikeuden saaminen ilman käyttäjää (daemon-palvelu) ja sovelluksen käyttöoikeuksia](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v2.0 – OAuth 2.0 -asiakastietojen kulku](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 Kielletty virhe: Salasanan vaihtaminen**

Tällä hetkellä ei ole sovellusten käyttöoikeus daemonin palvelussa käyttöoikeuksia, jotka sallivat käyttäjien salasanojen vaihtamisen. Näitä ohjelmointirajapintoja tuetaan vain vuorovaikutteisten valtuutettujen koodivirtojen avulla kirjautuneen järjestelmänvalvojan kanssa.

- [Microsoft Graphin käyttöoikeudet](https://docs.microsoft.com/graph/permissions-reference)

**403 Kielletty: Onko käyttäjällä käyttöoikeus ja onko hänellä käyttöoikeus?**

Microsoft Graph arvioi valtuutetuissa koodivirroissa, onko pyyntö sallittu sovellukseen myönnettyjen käyttöoikeuksien ja kirjautuneen käyttäjän käyttöoikeuksien perusteella. Yleensä tämä virhe tarkoittaa, että käyttäjällä ei ole järjestelmänoikeutta tehdä pyyntöä eikä käyttäjällä ei ole käyttöoikeutta tietoihin, joita hän voi käyttää. Vain käyttäjät, joilla on tarvittavat käyttöoikeudet, voivat tehdä pyynnön onnistuneesti.

**403 Kielletty: Oletko valinnut oikean resurssien ohjelmointirajapinnan?**

Api-palvelut, kuten Microsoft Graph tarkistavat, että vastaanottaneen käyttöoikeustietueen oletusarvo (käyttäjäryhmä) vastaa odottamaansa arvoa, ja jos näin ei ole, näyttöön tulee 403 Kielletty-virhe. Yleinen virhe, joka aiheuttaa tämän virheen, yrittää käyttää Azure AD Graph -ohjelmointirajapintojen, Outlook-ohjelmointirajapintojen tai SharePoint- tai OneDrive-ohjelmointirajapintojen hankkimaa tunnusta Microsoft Graphin kutsumisen (tai päinvastoin). Varmista, että sovellus hankkii resurssin (tai laajuuden), joka vastaa sovelluksen kutsumaa ohjelmointirajapintaa.

**400 Virheellinen pyyntö tai 403 Kielletty: Noudattaako käyttäjä organisaation ehdollisia käyttöoikeuskäytäntöjä?**

Organisaation varmenteiden myöntäjäkäytäntöjen mukaan käyttäjä, joka käyttää Microsoft Graph -resursseja sovelluksen kautta, saattaa olla haasteena lisätietoja, joita ei ole alun perin hankitussa sovelluksen käyttöoikeustietueessa. Tässä tapauksessa sovellus saa 400 -virheen *interaction_required* access-tunnusoston tai 403:n *insufficient_claims* Microsoft Graphia kutsuttaessa. Kummassakin tapauksessa virhevastaus sisältää lisätietoja, jotka voidaan esittää päätepisteille, jotta käyttäjä voi saada lisätietoja (kuten monimenetelmäisen todentamisen tai laitteen rekisteröinnin).

- [Ehdollisten access-haasteiden käsitteleminen MSAL:n avulla ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Azure Active Directoryn ehdollisen käytön opas kehittäjälle](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide) käyttö
