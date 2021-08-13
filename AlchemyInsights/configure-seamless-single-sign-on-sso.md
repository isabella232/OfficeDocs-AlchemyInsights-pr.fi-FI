---
title: Saumattoman kertakirjautumisen määrittäminen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004344"
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: 62f667cccd0761e081b3f651709fadfec12500e76fd8e30b8649a28e99001e4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966034"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Saumattoman kertakirjautumisen määrittäminen

**Sovellusten määrittäminen**

1. Sinun pitäisi saada arvot sovelluksen toimittajalta. Voit kirjoittaa arvot manuaalisesti tai ladata metatietotiedoston kenttien arvon poimimista varten.
2. Monet sovellukset on jo esiasennettu toimimaan Azure AD:n kanssa. Nämä sovellukset on lueteltu sovellusvalikoimassa, jota voit selata, kun lisäät sovelluksen Azure AD -vuokraajaan. [Pika-aloitussarjan avulla](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) voit käsitellä prosessia.
3. Jos haluat luoda sovelluksen, joka ei ole valikoima, napsauta + Luo **oma** sovellus -painiketta ja anna sovellukselle nimi.
    - Oletusarvoisesti se valitsee Integroi **kaikki muut sovellukset,** joita et löydä valikoimasta, joka on oikea vaihtoehto ei-valikoiman sovelluksille.
    - Kun olet **painanut Luo** sovelluksen nimen lisäämisen jälkeen, sovellus luo uuden yrityssovelluksen, joka ei ole valikoima.
    - Tämän jälkeen voit siirtyä **Kertakirjaus-kohtaan** Sovelluksen hallinta -kohdassa, ja näet erilaisia menetelmiä sen käyttöönotmiseksi ympäristössäsi. 

**Saumattoman SSO:n määrittäminen tietylle sovellukselle**

Valikoimassa olevia sovelluksia varten löydät yksityiskohtaiset, vaiheittaiset ohjeet. Pääset vaiheisiin selaamalla sovellusten määritysten opetusohjelmien luetteloa [SaaS-sovellusmääritysten opetusohjelmissa.](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)

**SAML-pohjaisen SSO:n määrittäminen**

1. [Pika-aloitus: SAML-pohjaisen kertakirjautumisen (SSO) luominen Azure Active Directory (Azure AD) -vuokraajassa.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)
2. Lisätietoja SAML-pohjaisen kertakirjauksesi vaihtoehdosta on kohdassa [SAML-pohjaisen kertakirjauksesi ymmärtäminen.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)
3. Lisätietoja SAML 2.0 :n todennuspyynnöistä ja vastauksista, joita Azure Active Directory (Azure AD) tukee Single Sign-On (SSO) -todennusta varten, on kohdassa [Yksittäinen Sign-On SAML-protokolla.](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
4. Lisätietoja SAML-pohjaisen kertakirjautumisen (SSO) luomiseen ja määrittämiseen sovellukselle Azure Active Directory (Azure AD) -sovelluksessa Microsoft Graph -ohjelmointirajapinnan avulla on kohdassa [SAML-pohjaisen](https://docs.microsoft.com/graph/application-saml-sso-configure-api)kertakirjautumisen määrittäminen sovellukselle Microsoft Graph -ohjelmointirajapinnan avulla.
5. Lisätietoja Siitä, miten Azure AD käyttää SAML-protokollaa, on kohdassa [SAML-Microsoftin käyttäjätietoympäristö SAML-protokollan käyttö.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)

**Tunnusten ja vaateiden määrittäminen**

1. [Ohjeet: saml-tunnuksessa myönnettyjen vaateiden mukauttaminen yrityssovelluksia varten.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)
2. Lisätietoja väiteiden määrittämisestä PowerShellin avulla on kohdassa How [to: Customize claims emitted inkens for a specific app in a tenant (Preview).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
3. Lisätietoja valinnaisten vaateiden määrittämisestä on [kohdassa How to: Provide optional claims to your app (Valinnaisten vaateiden tarjoaminen sovellukseen).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
4. Lisätietoja hakemistorakenteen laajennusmääritteiden käyttämisestä käyttäjien tietojen lähettämiseen sovelluksiin tunnusväitteissä on kohdassa Hakemistorakenteen [laajennusmääritteiden käyttäminen vaateissa.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions)
5. Lisätietoja tunnusten elinkaaren määrittämisestä on kohdassa Määritettävissä olevat tunnusten [elinkaari Microsoftin käyttäjätietoympäristö (esikatselu).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. [Määritä tunnusten elinkaaren käytännöt (esikatselu)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) – Tässä artikkelissa esikatsellaan yleistä käytäntöskenaariota, jonka avulla voit määrittää uusia sääntöjä tunnuksen elinkaaren aikana. Tässä esimerkissä opit luomaan käytännön, joka edellyttää, että käyttäjät todennetaan useammin verkkosovelluksessa.

**SSO-määritysten vianmääritys**

- Katso usein kysyttyjä kysymyksiä Azure Active Directory Seamless Single Sign-On (Seamless SSO) Azure Active Directory Seamless Single Sign-On: Frequently asked questions (Saumaton kertakirjautuminen: [usein kysytyt kysymykset).](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq)
- Katso vianmääritystietoja yleisistä Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO) Azure Active Directory -kertakirjautumisen [vianmäärityksestä.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)
