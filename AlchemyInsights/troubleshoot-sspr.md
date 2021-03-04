---
title: SSPR:n vianmääritys
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429721"
---
# <a name="troubleshoot-sspr"></a>SSPR:n vianmääritys

**Minulla on ongelmia salasanan palauttamisen määrittämisessä**

- Jos olet järjestelmänvalvoja ja haluat, miten omatoiminen salasanan vaihto otetaan käyttöön, katso [ohjeet SSPR:n](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)käyttöönottamisen opetusohjelmasta organisaation salasanan palauttamisen määrittämiseen. Voit myös tarkistaa [käyttöoikeusvaatimukset.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) Sinulla on oltava vähintään yksi käyttöoikeus määritettynä organisaatiossasi.
    - **Vain pilvipalvelun käyttäjät** – mikä tahansa Office 365 (O365) maksettu SKU tai Azure AD Basic
    - **Pilvi- ja/tai** paikalliskäyttäjät – Azure AD Premium P1 tai P2, Enterprise Mobility + Security (EMS) tai Secure Productive Enterprise (SPE)
- Lisätietoja omatoimisen salasanan palauttamisesta on usein [kysytyissä kysymyksissä.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**Näyttöön tulee virhesanoma**

Tässä artikkelissa on yleisiä virheitä ja niiden ratkaisuja: [Omatoiminen salasanan](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support) vaihtaminen -vianmääritys

**Minulla on ongelmia salasanan palautuskäytännön kanssa**

- Jos salasanan palautuskäytäntö ei toimi odotetulla tavalla tai jos sinulla on kysyttävää salasanan palautuskäytännöistä, lue tämä artikkeli: Salasanakäytännöt ja [-rajoitukset Azure Active Directoryssa.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)
- Salasanan palautuskäytännöt eivät koske järjestelmänvalvojille. Microsoft ottaa käyttöön vahvan kaksiportaisen salasanan palautuskäytännön kaikissa Azure-järjestelmänvalvojan roolissa. Varmista, että testaat käyttäjää, joka ei ole järjestelmänvalvoja. Lisätietoja järjestelmänvalvojan palautuskäytäntöön on tässä artikkelissa: Järjestelmänvalvojan [palautuskäytäntöjen erot.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**En halua käyttäjien rekisteröitävän muita suojaustietoja salasanan palauttamista varten**

Voit lisätä käyttäjien tiedot (sähköposti- ja puhelinmääritteet) valmiiksi ohjelmointirajapinnan, PowerShellin tai Azure AD Connectin avulla. Lue lisätietoja seuraavasti:

- [Salasanan palauttamisen käyttöönotto ilman, että käyttäjien on rekisteröidyttävä](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Mitä tietoja salasanan nollaaminen käyttää](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Haluan, että käyttäjät rekisteröivät lisäsuojaustietonsa salasanan palauttamista varten**

1. Anna käyttäjien rekisteröidä suojaustietonsa omatoimista salasanan vaihtoa varten ohjaamalla heidät [aka.ms/ssprsetup.](https://mysignins.microsoft.com/security-info)
1. Kun käyttäjä (käyttäjä tai järjestelmänvalvoja) täyttää tiedot, ohjaa käyttäjä [aka.ms/sspr](https://passwordreset.microsoftonline.com/) jotta käyttäjät voivat vaihtaa omat salasanansa.
1. Jos käyttäjillä on edelleen ongelmia, he ovat todennäköisimmin **liitettyjä käyttäjiä** tai salasanojen **hash-salasanojen synkronoinnissa.** Tämä tarkoittaa, että salasanan palautuspalvelussa on todennäköisesti ongelma.