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
ms.openlocfilehash: 9d8184efdc60befd359059c62ea3eb1a14ad7d2a20dade921d4a71e424f52033
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038955"
---
# <a name="troubleshoot-sspr"></a>SSPR:n vianmääritys

**Minulla on ongelmia salasanan palauttamisen määrittämisessä**

- Jos olet järjestelmänvalvoja ja etsit ohjeita omatoimista salasanan vaihtoa varten, katso lisätietoja [ohjevideosta SSPR:n](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)käyttöönottamisen käyttöönottajille organisaation salasanan palauttamisen määrittämiseksi. Voit myös tarkastella [käyttöoikeusvaatimuksia.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) Organisaatiossa on oltava määritettynä vähintään yksi käyttöoikeus.
    - **Vain pilvikäyttäjät** – mikä tahansa Office 365 (O365) maksettu SKU tai Azure AD Basic
    - **Pilvi- ja/tai paikalliskäyttäjät** – Azure AD Premium P1 tai P2, Enterprise Mobility + Security (EMS) tai Secure Productive Enterprise (SPE)
- Lisätietoja omatoimisen salasanan palauttamisesta on usein [kysytyissä kysymyksissä.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**Saan virhesanoman**

Tässä artikkelissa on yleisiä virheitä ja niiden ratkaisuja: [Omatoiminen salasanan vaihtotoiminnon vianmääritys](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Minulla on ongelmia salasanan vaihtokäytännön kanssa**

- Jos salasanan palautuskäytäntö ei toimi odotetulla tavalla tai jos sinulla on kysyttävää salasanan vaihtokäytännöistä, lue tämä artikkeli: Salasanan vaihtokäytäntöjen ja [-rajoitusten Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)
- Salasanan palautuskäytännöt eivät koske järjestelmänvalvojille. Microsoft ottaa käyttöön vahvan kaksiportaisen salasanan palautuskäytännön kaikissa Azure-järjestelmänvalvojan roolissa. Varmista, että testaat tietoja käyttäjän kanssa, joka ei ole järjestelmänvalvoja. Lisätietoja järjestelmänvalvojan palautuskäytäntöön on tässä artikkelissa: Järjestelmänvalvojan [palauttamista koskevat käytännön erot.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**En halua, että käyttäjät rekisteröivät muita suojaustietoja salasanan nollaamista varten**

Voit lisätä käyttäjille valmiiksi tietoja (sähköpostin ja puhelimen määritteet) ohjelmointirajapinnan, PowerShellin tai Azure AD:n Näyttöyhteys. Lue ohjeet tähän:

- [Salasanan palauttamisen käyttöönotto ilman, että käyttäjien on rekisteröidyttävä](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Mitä tietoja salasanan nollaaminen käyttää](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Haluan, että käyttäjät rekisteröivät muut suojaustietonsa salasanan nollaamista varten**

1. Käyttäjät rekisteröivät suojaustietonsa omatoimista salasanan vaihtoa varten ohjaamalla heidät [aka.ms/ssprsetup.](https://mysignins.microsoft.com/security-info)
1. Kun käyttäjä (käyttäjä tai järjestelmänvalvoja) on täytetty, ohjaa käyttäjä [aka.ms/sspr](https://passwordreset.microsoftonline.com/) jotta käyttäjät voivat vaihtaa omat salasanansa.
1. Jos käyttäjillä on edelleen ongelmia, he ovat todennäköisimmin **liitettyjä käyttäjiä** tai **salasanojen hash-salasanojen synkronoinnissa.** Tämä tarkoittaa, että salasanan kirjoituspalvelussa on todennäköisesti ongelma.