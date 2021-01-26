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
ms.openlocfilehash: 2ef90b54ce222a06740e05891fabe87b6565cb14
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/25/2021
ms.locfileid: "49984539"
---
# <a name="application-errors"></a>Sovellusvirheet

Etsitkö tietoja Azure Active Directory (Azure AD) -suojaustunnuspalvelusta (STS) palautetuista **AADSTS-virhekoodeista?** Lue [Azure AD -todennuksen ja valtuutuksen virhekoodien](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) avulla AADSTS-virheen kuvaukset, korjaukset ja joitakin ehdotettuja vaihtoehtoisia ratkaisuja.

Valtuutusvirheet voivat johtua useista eri ongelmista, joista useimmat luovat 401- tai 403-virheen. Esimerkiksi seuraavat voivat johtaa valtuutusvirheisiin:

- Virheelliset [käyttöoikeustietueiden hankintavirrat](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- Huonosti määritetyt [käyttöoikeuksien laajuudet](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- Suostumuksen [puute](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Jos haluat ratkaista yleisiä valtuutusvirheitä, kokeile alla olevia ohjeita, jotka vastaavat läheisimmin vastaanottamiasi virheitä. Useita voi olla voimassa.

**401 Luvaton virhe: Kelpaako tunnus?**

Varmista, että sovelluksesi esittää kelvollisen Käyttöoikeustietueen Microsoft Graphiin osana pyyntöä. Tämä virhe tarkoittaa usein sitä, että käyttöoikeustietue saattaa puuttua HTTP-todennuspyynnön otsikosta tai että tunnus on virheellinen tai vanhentunut. On erittäin suositeltavaa käyttää [Microsoftin todennuskirjastoa (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) käyttöoikeustietueiden hankintaan. Lisäksi tämä virhe voi ilmetä, jos yrität käyttää henkilökohtaiselle Microsoft-tilille myönnettyä delegoitua käyttöoikeustietueen avulla ohjelmointirajapintaa, joka tukee vain työ- tai koulutilejä (organisaatiotilit).

**403 Kielletty -virhe: Oletko valinnut oikeat käyttöoikeudet?**

Tarkista, että olet pyytänyt oikeita käyttöoikeuksia sovelluspuheluiden Microsoft Graph -ohjelmointirajapintojen perusteella. Suositellut järjestelmänvalvojan oikeudet on annettu kaikissa Microsoft Graph -ohjelmointirajapinnan ohjeaiheissa. Lisäksi käyttäjän tai järjestelmänvalvojan on myönnettävä nämä käyttöoikeudet sovellukseen. Käyttöoikeuksien myöntäminen tapahtuu yleensä suostumussivulla tai myöntämällä käyttöoikeuksia Azure Portal -sovelluksen rekisteröintilevyn avulla. Valitse **sovelluksen** Asetukset-sovelluksesta **Pakolliset käyttöoikeudet** ja valitse sitten **Myönnä käyttöoikeuksia.**

- [Microsoft Graphin käyttöoikeudet](https://docs.microsoft.com/graph/permissions-reference) 
- [Tietoja Azure AD:n käyttöoikeuksista ja suostumuksesta](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 Kielletty-virhe: Hankkiko sovellus tunnuksen, joka vastaa valittuja käyttöoikeuksia?**

Varmista, että pyydettyjen tai myönnettyjen käyttöoikeuksien tyyppi vastaa sovelluksen hankkimaa käyttöoikeustietuetyyppiä. Saatat pyytää ja myöntää sovelluksen käyttöoikeuksia, mutta käytät delegoituja vuorovaikutteisia koodinkulkutunnuksia asiakkaan tunnistetietojenkulkutunnusten sijaan tai pyydät ja myöntävät delegoituja käyttöoikeuksia, mutta käytät asiakkaan tunnistetietovuotunnuksia valtuutisten kooditunnusten sijaan.

- [Käyttöoikeuden saaminen käyttäjien puolesta ja delegoidut käyttöoikeudet](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v2.0 - OAuth 2.0 -valtuutuskoodin kulku](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Käyttöoikeuden saaminen ilman käyttäjää (daemon-palvelu) ja sovelluksen käyttöoikeuksia](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v2.0 – OAuth 2.0 -asiakasohjelman tunnistetietojen kulku](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 Kielletty -virhe: salasanan vaihtaminen**

Tällä hetkellä ei ole sovelluksen käyttöoikeus daemon-palvelun käyttöoikeuksia, jotka sallivat käyttäjien salasanojen vaihtamisen. Näitä ohjelmointirajapintoja tuetaan vain vuorovaikutteisten valtuutetuissa koodivirroissa kirjautuneen järjestelmänvalvojan kanssa.

- [Microsoft Graphin käyttöoikeudet](https://docs.microsoft.com/graph/permissions-reference)

**403 Kielletty: Onko käyttäjällä käyttöoikeus ja onko hänellä käyttöoikeus?**

Microsoft Graph arvioi valtuutetuissa koodivirroissa, onko pyyntö sallittu sovellukseen myönnettyjen käyttöoikeuksien ja kirjautuneen käyttäjän käyttöoikeuksien perusteella. Yleensä tämä virhe tarkoittaa, että käyttäjällä ei ole tarpeeksi käyttöoikeuksia pyynnön suorittamiseen tai että käyttäjällä ei ole käyttöoikeutta tietoihin, joita hän käyttää. Vain käyttäjät, joilla on tarvittavat käyttöoikeudet, voivat tehdä pyynnön onnistuneesti.

**403 Kielletty: Oletko valinnut oikean resurssirajapinnan?**

Api-palvelut, kuten Microsoft Graph, tarkistavat, että vastaanottaneen käyttöoikeustietueen oletusarvo (käyttäjäryhmä) vastaa itse odottamaansa arvoa, ja jos näin ei ole, näyttöön tulee 403 Kielletty-virhe. Yleinen virhe, joka aiheuttaa tämän virheen, yrittää käyttää Azure AD Graphin ohjelmointirajapintojen, Outlook-ohjelmointirajapintojen tai SharePointin/OneDriven ohjelmointirajapintojen tunnuksia Microsoft Graphiin kutsumaan (tai päinvastoin). Varmista, että sovellus hankkii resurssin (tai laajuuden) tunnuksen, joka vastaa sovelluksen kutsumaa ohjelmointirajapintaa.

**400 Virheellinen pyyntö tai 403 Kielletty: Noudattaako käyttäjä organisaation ehdollisia käyttöoikeuskäytäntöjä?**

Organisaation varmenteiden myöntäjäkäytäntöjen perusteella käyttäjä, joka käyttää Microsoft Graph -resursseja sovelluksen kautta, voi olla haastavaa saada lisätietoja, joita ei ole alun perin hankitussa käyttöoikeustietueessa. Tässä tapauksessa sovelluksesi saa virheilmoituksen 400 *ja interaction_required* tunnuksen hankintaan tai 403:een, *jossa on insufficient_claims* virhe, kun soitat Microsoft Graphiin. Kummassakin tapauksessa virhevastaus sisältää lisätietoja, jotka voidaan esittää päätepisteille, jotta käyttäjä voi saada lisätietoja (kuten monimenetelmäisen todentamisen tai laitteen rekisteröinnin).

- [Ehdollisten access-haasteiden käsittely MSAL:n avulla ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Kehittäjän ohjeet Azure Active Directoryn ehdolliseen käyttöön](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
