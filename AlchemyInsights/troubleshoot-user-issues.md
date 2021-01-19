---
title: Käyttäjäongelmien vianmääritys
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7813"
- "9004358"
ms.openlocfilehash: d9964e50bdea0c41ac14ab3783b579034b5f2c8c
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901036"
---
# <a name="announcements"></a>Ilmoitukset

Noudata Googlen ohjeita yhteensopivuuden testaamiseen sen testaamiseksi, vaikuttaako sovelluksiin tämä ongelma. Googlen ohjeet ovat saatavilla https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support .

Varmista, että käytät järjestelmän verkkonäkymää tai järjestelmäselainta, kun kirjaudut sisään käyttäjiisi kuluttaja-Google-tileillä. Lisätietoja on kohdassa Sovellukseen [kirjautumisongelmat vain Chrome-selaimella.](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)


**En voi luoda uutta käyttäjää Azure AD -hakemistossa**

Jos haluat tehdä vianmäärityksen siitä, että uutta käyttäjää ei voi luoda Azure AD:ssä, toimi seuraavasti:

1. Varmista, että sinulla on oikeus luoda uusi peruskäyttäjä. Vain yleinen järjestelmänvalvoja tai käyttäjän järjestelmänvalvojan rooli Azure Active Directoryssa (AD) voi luoda uuden peruskäyttäjän. Jos et ole jossakin näistä rooleista, pyydä järjestelmänvalvojaa lisäämään sinut näihin rooleihin tai luomaan uusi käyttäjätili.
2. Varmista, että käyttäjänimi on toimialueessa, joka on vahvistettu Azure AD:ssäsi. Jos Azure AD:ssä ei ole vahvistettuja mukautettuja toimialuenimiä, voit käyttää Azure AD:n alkuperäistä toimialuetta, joka päättyy *.onmicrosoft.com.
3. Varmista, että käyttäjänimi on toimialueella, jota ei ole liitetty Azure AD:han paikallisesta AD:stä. Käyttäjiä ei voi lisätä pilvipalveluun toimialuenimillä, jotka on liitetty paikallisesti.
4. Varmista, että toisella käyttäjällä tai yhteyshenkilöllä ei ole vielä käyttäjänimiä, jonka haluat määrittää uudelle käyttäjälle. Käyttäjien nimien on oltava yksilöllisiä Azure AD:ssä.
5. Tutustu [Azure AD:n rooleihin ja](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) järjestelmänvalvojiin Azure AD:ssä.
6. Katso Azure [AD:n](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) toimialuenimet.
7. Tarkista [valvontalokit,](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) jos haluat nähdä tarkempia tietoja äskettäin luodusta tai poistetuksi käyttäjästä, kuten toiminnon suorittavasta henkilöstä ja milloin.
8. Lisätietoja uusien käyttäjien lisäämisestä on ohjeaiheessa Uuden käyttäjän luominen [Azure-portaalissa Azure AD:ssä.](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
9. Lisätietoja järjestelmänvalvojan roolin käyttöoikeuksista Azure AD:ssä on [Azure AD:n järjestelmänvalvojan rooleissa.](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
10. Lisätietoja käyttäjän luomisesta Azure AD Powershellin avulla on ohjeaiheessa [Azure AD PowerShell ja luo uusi käyttäjä.](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser)

**Ongelma omatoimisissa rekisteröitynystoiminnissa**

Tee omatoimista rekisteröitymista koskevien ongelmien vianmääritys seuraavasti:

1. Jos haluat käyttää omatoimista rekisteröitymistä sovelluksissasi, ota ensin omatoiminen rekisteröityminen käyttöön vuokraajassasi. 
2. Jos haluat, että sovellus tukee omatoimista rekisteröityä, lisää se käyttäjän työnkulkuun. Kun seuraavan kerran siirryt sovelluksen kirjautumissivulle, näet vaihtoehdon **_Ei tiliä? Luo sellainen!_* _. Tämä käynnistää omatoiminen rekisteröitymisprosessin.
3. Lisätietoja omatoimisen rekisteröityminen organisaation käyttöön Azure AD:ssä on kohdassa [Azure AD:n](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup)omatoiminen rekisteröityminen.
4. Kun liität käyttäjän työnkulun yhteen tai useampiin sovelluksiin, käyttäjät, jotka vierailevat sovelluksessa, voivat rekisteröityä ja hankkia vierastilin käyttäjän työnkulussa määritettyjen asetusten avulla. Lisätietoja vierastilin rekisteröimisestä ja saamisesta on vieraskäyttäjien omatoimisissa [rekisteröitymispalveluissa.](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow)

_ *Ongelma ulkoisen käyttäjän kutsuminen**

Voit tehdä ulkoisen käyttäjän kutsumista koskevien ongelmien vianmäärityksen seuraavasti:

Varmista, että lähetät käyttäjän kutsun sähköpostiosoitteeseen, joka vastaa nimeä, jolla käyttäjä kirjautuu sisään. Jos lähetät kutsun käyttäjän välityspalvelimen sähköpostiosoitteeseen, käyttäjä ei voi lunastaa sitä. Lisätietoja on [Azure AD B2B :n ohjeissa.](https://docs.microsoft.com/azure/active-directory/external-identities/)

**Käyttöoikeuksia ei voi määrittää käyttäjälle**

Voit määrittää käyttäjälle käyttöoikeuksia koskevia ongelmia seuraavasti:

1. Jos haluat hallita käyttöoikeuksia, varmista, että käytät tiliä, jossa on jokin tarvittavista järjestelmänvalvojan rooleista: yleinen järjestelmänvalvoja, käyttöoikeuksien järjestelmänvalvoja tai käyttäjän järjestelmänvalvoja. Voit tarkistaa käyttäjän roolin käyttäjän **terien** Hakemistorooli-välilehdessä.
2. Jos käytät Azure-portaalia ja käyttöoikeuksien määritys epäonnistuu, napsauta oikeassa yläkulmassa olevaa ilmoitusta. Tämä avaa terän, jossa on tietoja siitä, mikä meni vikaan. Useimmissa tapauksissa tämä riittää ongelman ymmärtäminen ja ratkaiseminen.
3. Ennen kuin käyttäjälle voidaan määrittää käyttöoikeus, varmista, että **Käyttösijainti-ominaisuus** on määritetty käyttäjälle. Tarkista, että käyttäjä on määrittänyt tämän **ominaisuuden,** tarkastelemalla profiilivälilehteä käyttäjän terissä.
4. Varmista, että määritettävälle tuotteelle on riittävästi käyttöoikeuksia. Näet azure-portaalissa käytettävissä olevien käyttöoikeuksien määrän Azure [Active Directory -> -> kaikki tuotteet.](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products)
5. Käyttäjällä voi jo olla toinen käyttöoikeus, jonka palvelut ovat ristiriidassa määritettävän uuden käyttöoikeuden kanssa. Jos käyttäjällä on esimerkiksi käytössä Exchange Online (palvelupaketti 1) -palvelu, et voi määrittää käyttöoikeutta Exchange Onlinessa (palvelupaketti 2). Voit sallia uuden käyttöoikeuden määrityksen poistamalla yhden palveluista käytöstä. Jos käytät Azure-portaalia tai PowerShellin  cmdlet-komentoja, ongelman tiedot -sivulla luetellaan ne palvelut, jotka aiheuttavat ristiriidan.
6. Jos yrität poistaa käyttöoikeuden ja se epäonnistuu, käyttäjällä voi olla muita käyttöoikeuksia, jotka riippuvat palveluista, jotka yrität poistaa. Jos käytät Azure-portaalia tai PowerShellin cmdlet-komentoja, virhesanomassa on luettelo niistä palveluista, jotka ovat riippuvaisia.
7. Jos haluat tietää, miksi käyttäjä on lisännyt tai poistanut käyttöoikeuden (esimerkiksi se, kuka muu organisaatiossasi on voinut tehdä muutoksia), tarkista valvontalokit. Määritä suodatin näyttämään **kaikki muutokset,** mukaan lukien "toimija", joka on suorittanut ne.
8. Jos käytät Exchange Onlinea, jotkin vuokraajan käyttäjät on voitu määrittää virheellisesti samalla välityspalvelimen osoitearvolla. Tällöin saatat nähdä yleisiä virhesanomia, kun käyttöoikeustoiminto epäonnistuu. [Tässä artikkelissa](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) on lisätietoja tästä ongelmasta, mukaan lukien tiedot yhteyden muodostamisesta [Exchange Onlineen Etä-PowerShellin avulla.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell) Määritä, mitkä vuokraajan käyttäjät sisältävät saman välityspalvelimen osoitteen, suorittamalla tämän Exchange Onlinen cmdlet-komennon:

Suorita

Get-Recipient | jossa {$_. EmailAddresses -match <user principal name> } | fL Name, RecipientType,emailaddresses





