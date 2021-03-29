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
ms.openlocfilehash: bd3873c2db1b8d548f81d531a8bf5747130fe761
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402264"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Saumattoman kertakirjautumisen määrittäminen

**Sovellusten määrittäminen**

1. Sinun pitäisi saada arvot sovelluksen toimittajalta. Voit kirjoittaa arvot manuaalisesti tai ladata metatietotiedoston kenttien arvon poimimista varten.
2. Monet sovellukset on jo määritetty toimimaan Azure AD:n kanssa. Nämä sovellukset on lueteltu sovellusvalikoimassa, jota voit selata, kun lisäät sovelluksen Azure AD -vuokraajaan. [Pika-aloitussarja opastaa](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) sinua prosessissa.
3. Jos haluat luoda ei-valikoimasovelluksen, voit napsauttaa + Luo **oma** sovellus -painiketta ja antaa sovellukselle nimen.
    - Oletusarvoisesti se valitsee Integroi **kaikki muut** sovellukset, joita et löydä valikoimasta, joka on oikea vaihtoehto ei-valikoimasovelluksille.
    - Kun painat **Luo** sovelluksen nimen lisäämisen jälkeen, sovellus luo uuden yrityssovelluksen, joka ei ole valikoima.
    - Tämän jälkeen voit siirtyä **Kertakirjaus-kohtaan** sovelluksen hallinta -kohdassa, ja näet erilaisia tekniikoita sovelluksen käyttöönotetmiseksi ympäristössäsi. 

**Saumattoman SSO:n määrittäminen tietylle sovellukselle**

Valikoimassa olevia sovelluksia varten löydät yksityiskohtaiset, vaiheittaiset ohjeet. Pääset vaiheisiin selaamalla sovellusten määritysten opetusohjelmien luetteloa [SaaS-sovelluksen määritysten opetusohjelmissa.](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)

**SAML-pohjaisen SSO:n määrittäminen**

1. [Pika-aloitus: SAML-pohjaisen kertakirjautumisen (SSO)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)määritetään Azure Active Directory (Azure AD) -vuokraajan sovellukselle.
2. Lisätietoja SAML-pohjaisen kertakirjauksesi vaihtoehdosta on kohdassa [SAML-pohjaisen kertakirjautimen ymmärtäminen.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)
3. Lisätietoja SAML 2.0 -todennuspyynnöistä ja vastauksista, joita Azure Active Directory (Azure AD) tukee Single Sign-On (SSO) -protokollaa varten, on kohdassa [Single Sign-On SAML -protokolla.](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
4. Lisätietoja SAML-pohjaisen kertakirjautumisen (SSO) luomiseen ja määrittämiseen sovellukselle Azure Active Directoryssa (Azure AD) Microsoft Graph API:n avulla on kohdassa SAML-pohjaisen kertakirjautumisen määrittäminen [sovellukselle Microsoft Graph -ohjelmointirajapinnan avulla.](https://docs.microsoft.com/graph/application-saml-sso-configure-api)
5. Lisätietoja AZURE AD:n SAML-protokollan käytön käytöstä on kohdassa [Miten Microsoftin tunnistetietoympäristö käyttää SAML-protokollaa.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)

**Tunnusten ja vaateiden määrittäminen**

1. [Toiminta-ohjeet: yrityssovelluksissa SAML-tunnuksessa myönnettyjen vaateiden mukauttaminen.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)
2. Lisätietoja väiteiden määrittämisestä PowerShellin avulla on kohdassa How to: Customize claims [emitted inkens for a specific app in a tenant (Preview).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
3. Lisätietoja valinnaisten vaateiden määrittämisestä on [kohdassa Toiminta: Valinnaisten vaateiden tarjoaminen sovellukseen.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
4. Lisätietoja hakemistorakenteen laajennusmääritteiden käyttämisestä käyttäjien tietojen lähettämiseen sovelluksiin tunnuksen vaateissa on kohdassa [Hakemistorakenteen laajennusten määritteiden käyttäminen vaateissa.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions)
5. Lisätietoja tunnusten elinkaaren määrittämisestä on kohdassa Määritettävissä olevat [tunnusten elinkaarit Microsoftin käyttäjätietoympäristössä (esikatselu).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. [Määritä tunnusten käyttöajan](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) käytännöt (esikatselu) – Tässä artikkelissa käymme läpi yhteisen käytäntöskenaarion, jonka avulla voit määrittää uusia sääntöjä tunnusten elinkaaren osalta. Tässä esimerkissä opit luomaan käytännön, joka edellyttää, että käyttäjät todennetaan useammin verkkosovelluksessa.

**SSO-kokoonpanon vianmääritys**

- Usein kysyttyjä kysymyksiä Azure Active Directory Seamless Single Sign-On (Seamless SSO) -tallennustilasta [on Azure Active Directory Seamless Single Sign-On -sivulla: Usein kysytyt kysymykset.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq)
- Lisätietoja Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO) -kertakirjautumisen yleisistä ongelmista on ohjeaiheessa Azure Active Directoryn saumattoman [kertakirjautumisen vianmääritys.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)
