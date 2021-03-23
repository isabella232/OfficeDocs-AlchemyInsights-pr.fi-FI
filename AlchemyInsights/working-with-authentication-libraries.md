---
title: Todennuskirjastojen käyttäminen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035285"
---
# <a name="working-with-authentication-libraries"></a>Todennuskirjastojen käyttäminen

Voit ratkaista Microsoftin todennuskirjaston (MSAL) ongelman noudattamalla seuraavia suositeltuja ohjeita:

1. **MSAL:n käyttäminen:** [Microsoftin käyttäjätietojen alustojen todennuskirjastot](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) – Tässä artikkelissa kerrotaan Microsoftin todennuskirjaston tuesta useille sovellustyypeille. Se sisältää linkkejä kirjaston lähdekoodiin; mistä saat paketin sovelluksen projektia varten ja tukeeko kirjasto käyttäjän kirjautumista (todennusta), suojattujen verkkorajapintojen (valtuutuksen) käyttö vai molemmat.

2. **Todennuksen** vianmääritys: MSAL tukee useita todennusvirtoja käytettäväksi eri sovellusskenaarioissa. Sen mukaan, miten asiakassovellus on luotu, MSAL voi käyttää vähintään yhtä Microsoftin käyttäjätietoympäristön tukemista todennusvirroista. Nämä työnkulut voivat tuottaa monenlaisia tunnuksia ja valtuutuskoodeja, ja niiden toimiminen edellyttää erilaisia tunnuksia.

3. **Access Tokens:** [Microsoft identity platform access tokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Learn how your API can validate and use the claims inside an access token. Kaikki tämän artikkelin ohjeet, paitsi jos ne on mainittu, koskevat vain rekisteröityjen ohjelmointirajapintojen tunnuksia. Se ei koske Microsoftin omistamien ohjelmointirajapintojen tunnuksia eikä tunnuksia voida käyttää sen tarkistamiseen, miten Microsoftin tunnistetietoympäristö myöntää tunnuksia luomaasi ohjelmointirajapintaan.

**Azure Active Directory -todennuskirjaston (ADAL) tuen päättyminen**

- **30. kesäkuuta 2020** alkaen uusia ominaisuuksia ei enää lisätä ADAL:een ja Azure AD Graphiin. Tarjoamme jatkossakin teknistä tukea ja suojauspäivityksiä, mutta emme enää tarjoa ominaisuuspäivityksiä.
- **30. kesäkuuta 2022** alkaen microsoft lopettaa ADAL: n ja Azure AD Graphin tuen, eikä se enää tarjoa teknistä tukea tai suojauspäivityksiä.
- Sovellukset, jotka käyttävät ADAL:tä nykyisissä käyttöjärjestelmäversioissa, toimivat edelleen tämän ajan kuluttua, mutta eivät saa *teknistä tukea tai suojauspäivityksiä.*
- Azure AD Graphia tämän jälkeen käyttävät sovellukset eivät ehkä enää saa vastauksia Azure AD Graph -päätepisteltä.

**ADAL-siirto**

- Suosittelemme päivittämään MSAL-versioon, jossa on uusimmat ominaisuudet ja suojauspäivitykset.
- Jos käytät Microsoft-sovelluksia, tiedät, että Microsoft on parhaillaan muuttamassa sovelluksiaan MSAL-sovelluksiin tuen päättymiseen mennessä, jotta ne hyötyvät MSAL:n käynnissä olevista suojaus- ja ominaisuusparannuksista.

1. [Lue ADAL:n usein kysytyt kysymykset.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Lue lisää siitä, miten voit siirtää sovelluksia käyttöympäristökohtaisesti.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance)
3. Jos sinulla on lisäkysymyksiä sovelluksen käyttöympäristön oppaan lukemisen jälkeen, voit julkaista sen [Microsoftin kysymysten ja](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) kysymysten&A -tunnisteella [azure-ad-adal-deprecation] tai avata ongelman kirjaston GitHub-säilössä. [MSAL-yleiskatsausartikkelin](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) Kielet  ja kehykset -osassa on linkkejä kunkin kirjaston repo-kohteeseen.
4. **Jos tarvitset apua ADAL-sovellusten** käytössä, suosittelemme tarkistamaan kaikki sovellusten lähdekoodit. Ota tarvittaessa yhteyttä itsenäisten ohjelmistotoimittajien (ISV) tai sovellustoimittajien käyttöön. Microsoftin tukipalvelu voi myös tarjota sinulle luettelon kaikista vuokraajan ei-Microsoft ADAL -sovelluksista.







