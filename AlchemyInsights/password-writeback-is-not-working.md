---
title: Salasanan takaisin kirjoittaminen ei toimi
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
- "9004595"
- "8210"
ms.openlocfilehash: 679dea6d488cf74f51baee2b3b498dc64b95530e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324920"
---
# <a name="password-writeback-is-not-working"></a>Salasanan takaisin kirjoittaminen ei toimi

**Minulla on ongelmia salasanan takaisin kirjoittamisen määrittämisessä**

- Salasanan takaisin kirjoittaminen on premium-ominaisuus.
- Varmista, että ymmärrät käyttöoikeusvaatimukset:
  - Sinulla on oltava vähintään yksi käyttöoikeus määritettynä organisaatiossasi
  - **Vain pilvikäyttäjät** – mikä tahansa Office 365 (O365) maksettu SKU tai Azure AD Basic
  - **Pilvi- ja/tai paikalliskäyttäjät** – Azure AD Premium P1 tai P2, Enterprise Mobility + Security (EMS) tai Secure Productive Enterprise (SPE)
    - Lisätietoja käyttöoikeusvaatimuksista on kohdassa [Azure AD:n omatoimista salasanan vaihtoa koskevat käyttöoikeusvaatimukset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Sinulla on vähintään yksi järjestelmänvalvojan tili ja yksi testikäyttäjätili, jolla on sopiva käyttöoikeus.
- Azure AD -palvelin on Näyttöyhteys toimialueen ohjausohjaimen emulaattoriin, jotta salasanan takaisin kirjoittaminen toimii. Voit määrittää Azure AD Näyttöyhteys käyttämään ensisijaista toimialueen ohjauskonetta  napsauttamalla Active Directory -synkronoinnin yhdistimen ominaisuuksia hiiren kakkospainikkeella ja valitsemalla sitten **määritä hakemisto-osiot.** Etsi sieltä toimialueen ohjauskoneen **yhteysasetusten osio** ja valitse valintaruutu, jossa on vain ensisijaiset **toimialueen ohjauskotimet.**
    **Huomautus:Jos** ensisijainen DC ei ole PDC-emulaattori, Azure AD Näyttöyhteys ottaa edelleen yhteyttä PDC:hen salasanan takaisinkirjaamista varten.
- Salasanan vaihtaminen on määritetty ja otettu käyttöön vuokraajassa. Lisätietoja on kohdassa Azure [AD -salasanojen palauttamisen salliminen käyttäjille.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Varmista, että salasanalla kirjoittamisen käyttöönottoon käytettävä järjestelmänvalvojan tili on pilvipalvelun järjestelmänvalvojan tili (luotu Azure AD:ssä eikä paikallisessa AD:ssä)
- Käytössäsi Windows Server 2008 R2:n, Windows Server 2012:n tai Windows Server 2012 R2:n paikallinen monipuuryhmäympäristö, johon on asennettu uusimmat Service Pack -paketit
- Sinulla on Azure AD Näyttöyhteys asennettuna ja olet valmistellut AD-ympäristön synkronointia varten pilvipalveluun. Ennen kuin testaat salasanan takaisin kirjoittaminen, varmista, että suoritat ensin täydellisen tuonnin ja täyden synkronoinnin sekä AD:stä että Azure AD:stä Azure AD:ssä Näyttöyhteys.
- Lisätietoja on kohdassa Täydet synkronoinnit ja täysi [tuonti Azure AD Näyttöyhteys](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Minulla on ongelmia salasanan takaisin kirjoittamisen yhteydessä**

1. Uusimman Azure AD -version lataaminen [ja Näyttöyhteys](https://www.microsoft.com/download/details.aspx?id=47594)
2. Palomuurin määritys: Azure AD Näyttöyhteys -työkalun (1.1.443 tai uudempi versio) on **lähtevien** HTTPS-yhteyksien käyttö:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Salli joutoyhteyksien säilyminen vähintään 2–3 minuutin ajan

**Minulla on edelleen ongelmia salasanan takaisin kirjoittamisen kanssa**

- Jos sinulla on edelleen ongelmia, kokeile poistaa salasanasuojauspalvelu käytöstä ja ottaa se uudelleen käyttöön Azure AD Näyttöyhteys työkalussa
- Lisätietoja on ohjeaiheessa Salasanan palautusten poistaminen käytöstä [ja ottaminen uudelleen käyttöön](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
