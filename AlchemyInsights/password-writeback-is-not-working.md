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
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243364"
---
# <a name="password-writeback-is-not-working"></a>Salasanan takaisin kirjoittaminen ei toimi

**Minulla on ongelmia salasanan takaisin kirjoittamisen määrittämisessä**

- Salasanan takaisin kirjoittaminen on premium-ominaisuus.
- Varmista, että ymmärrät käyttöoikeusvaatimukset:
  - Sinulla on oltava vähintään yksi käyttöoikeus määritettynä organisaatiossasi
  - **Vain pilvipalvelun käyttäjät** – mikä tahansa Office 365 (O365) maksettu SKU tai Azure AD Basic
  - **Pilvi- ja/tai** paikalliskäyttäjät – Azure AD Premium P1 tai P2, Enterprise Mobility + Security (EMS) tai Secure Productive Enterprise (SPE)
    - Lisätietoja käyttöoikeusvaatimuksista on kohdassa [Azure AD:n omatoimista salasanan vaihtoa koskevat käyttöoikeusvaatimukset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Sinulla on vähintään yksi järjestelmänvalvojan tili ja yksi testikäyttäjätili, jolla on jokin asianmukainen käyttöoikeus.
- Azure AD Connect on kytkettävä ensisijaiseen toimialueen ohjauskoneemulaattoriin, jotta salasanan palautus toimii. Voit määrittää Azure AD Connectin käyttämään ensisijaista toimialueen  ohjauskonetta napsauttamalla Active Directory -synkronointiyhdistimen ominaisuuksia hiiren kakkospainikkeella ja valitsemalla sitten **määritä hakemisto-osiot.** Etsi sieltä toimialueen ohjauskoneen **yhteysasetukset** -osio ja valitse ruutu, jossa on vain ensisijaiset **toimialueen ohjauskoneet.**
  > [!NOTE]
  > Jos ensisijainen DC ei ole PDC-emulaattori, Azure AD Connect ottaa edelleen yhteyttä PDC:hen salasanan palautusta varten.
- Salasanan vaihtaminen on määritetty ja otettu käyttöön vuokraajassa. Lisätietoja on kohdassa Azure [AD -salasanojen palauttamisen salliminen käyttäjille.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Varmista, että salasanan palautus otetaan käyttöön järjestelmänvalvojan tilillä pilvipalvelun järjestelmänvalvojan tilillä (luotu Azure AD:ssä, ei paikallisessa AD:ssä)
- Käytössäsi on yksittäinen tai usean puuryhmän AD-ympäristö, jossa on Windows Server 2008 R2, Windows Server 2012 tai Windows Server 2012 R2, johon on asennettu uusimmat Service Pack -paketit
- Sinulla on Azure AD Connect -työkalu asennettuna ja olet valmistellut AD-ympäristön synkronointia varten pilvipalveluun. Ennen kuin testaat salasanan takaisin kirjoittamisen, varmista, että suoritat ensin täydellisen tuonnin ja täyden synkronoinnin sekä AD:stä että Azure AD:stä Azure AD Connectissa.
- Lisätietoja on ohjeaiheessa Täyden synkronoinnin ja täyden [tuonnin luominen Azure AD Connectissa](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Minulla on ongelmia salasanan takaisin kirjoittamisen yhteydessä**

1. [Azure AD Connectin](https://www.microsoft.com/download/details.aspx?id=47594) uusimman version lataaminen ja ottaminen käyttöön
2. Palomuurin määritys: Azure AD Connect -työkalulla (1.1.443 ja sitä uudempi versio) on **lähtevien HTTPS-yhteyksien** käyttö:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Salli käyttämättömän yhteyden jatkuminen vähintään 2–3 minuutin ajan

**Minulla on edelleen ongelmia salasanan takaisin kirjoittamisen kanssa**

- Jos sinulla on edelleen ongelmia, kokeile poistaa salasanan palautuspalvelu käytöstä ja ottaa se uudelleen käyttöön Azure AD Connect -työkalussa.
- Lisätietoja on ohjeaiheessa Salasanan [palautusten poistaminen käytöstä ja ottaminen uudelleen käyttöön](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
