---
title: Ryhmäongelmien vianmääritys
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
- "7814"
- "9004358"
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/18/2021
ms.locfileid: "50713647"
---
# <a name="troubleshoot-group-issues"></a>Ryhmäongelmien vianmääritys

**Haluan määrittää ryhmän Azure AD -rooliin**

Voit määrittää Azure Active Directory (AD) -ryhmän Azure AD -rooliin seuraavasti:

1. Uuden ryhmän luominen – Uuden ryhmän luominen:

    a. Kirjaudu Azure AD -hallintakeskukseen järjestelmänvalvojan tai yleisen järjestelmänvalvojan käyttöoikeuksilla. 
    b. Valitse Azure Active Directory > ryhmät > Kaikki ryhmät > uusi ryhmä. 
    c. Luo ryhmä.

2. Määritä rooli ryhmälle joko ryhmän luomisen tai sen luomisen jälkeen.

    a. Jos haluat määrittää ryhmälle roolin ryhmän luomisen yhteydessä, voit määrittää ryhmälle azure AD -roolien vaihtopainikkeen ja luoda ryhmän.
    b. Jos haluat määrittää roolin ryhmälle sen luomisen jälkeen, siirry juuri luodun ryhmän Määritetyt roolit -välilehteen ja määritä rooli ryhmälle.

**Haluan hallita Azure AD -rooliin määritetyn ryhmän jäsenyyttä**

1. Oletusarvoisesti vain järjestelmänvalvoja ja yleinen järjestelmänvalvoja voivat estää oikeuksien laajentamisen muokkaamalla rooliin määritetyn ryhmän jäsenyyttä. He voivat kuitenkin määrittää omistajalle tällaisen ryhmän ja delegoida tämän tehtävän. Lisätietoja on pilvessä [roolimäärityksen hallintaan Azure Active Directoryssa.](https://docs.microsoft.com/azure/active-directory/roles/groups-concept)
2. Yleisiä kysymyksiä ja vianmääritysvihjeitä roolien määrittämiseen ryhmille Azure AD:ssä on kohdassa Pilviryhmille [määritettyjen roolien vianmääritys.](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)

**Dynaamiset ryhmät**

1. Jos et löydä käyttäjän sisäänrakennettuja määritteitä, varmista, että määrite on tuettujen ominaisuuksien luettelossa.
2. Jos etsit laitteen sisäänrakennettuja määritteitä, varmista, että määrite on laitemääritteiden luettelossa 
3. Valmiiden käyttäjän ja laitteen määritteiden lisäksi voit käyttää myös extension [attributes -määritteitä.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties) Kun olet synkronoinut laajennuksen määritteet paikallisesta Windows Server AD:stä tai yhdistetystä SaaS-sovelluksesta, määritteiden pitäisi näkyä säännön muodostimen avattavassa luettelossa. Mukautetun määritteen nimi löytyy hakemistosta kyselyllä käyttäjän määritteeseen PowerShellin avulla ja etsimällä määritteen nimeä. Näitä voidaan käyttää myös sääntöjen luomiseen säännön syntaksissa.
4. Varmista, että vuokraajassa on asianmukainen käyttöoikeus. Dynaamiset ryhmät edellyttävät, että vuokralaiselle on oltava Azure AD P1 Premium -käyttöoikeus. Tässä on luettelo Azure AD [-käyttöoikeussuunnitelmista.](https://azure.microsoft.com/pricing/details/active-directory/) Enterprise Mobility + Security -käyttöoikeussopimuksia voi käyttää [täällä.](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing)
5. Varmista, että dynaamisen ryhmän luovan käyttäjän rooli on yleinen järjestelmänvalvoja, intune-järjestelmänvalvoja, ryhmän järjestelmänvalvoja tai käyttäjän järjestelmänvalvoja.
6. Anna ryhmän täyttää aika. Vuokraajan koosta riippuen ryhmä voi kestää jopa 24 tuntia, ennen kuin populaaminen kestää ensimmäisen kerran tai säännön muutoksen jälkeen.
7. Lisätietoja on kohdassa Määritepohjaisten sääntöjen luominen [dynaamista ryhmän jäsenyyttä varten.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership)

**Minun on poistettava ryhmä**

1. Ryhmät voidaan poistaa hakemistosta käyttämällä Azure AD Powershell Remove-AzureADGroup cmdlet-komentoa.
2. Ennen kuin yrität poistaa synkronoidun ryhmän Azure AD:ssä, varmista, että olet poistanut kaikki määritetyt käyttöoikeudet virheiden välttämiseksi.
3. Lisätietoja ryhmien poistamisesta on ohjeaiheessa Määritetyn käyttöoikeuden ryhmän [poistaminen.](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license)

**Poistettu ryhmä on palautettava**

1. Jos Office 365 -ryhmä poistetaan, se voidaan palauttaa vain 30 päivää ennen pysyvää poistamista. Kun ryhmä on poistettu pysyvästi, sitä ei voi enää palauttaa. Lisätietoja ryhmien palauttamisesta [on täällä.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)
2. Tätä toimintoa ei tueta käyttöoikeusryhmissä ja jakeluryhmissä.
3. Varmista, että sinulla on oikeus palauttaa Office 365 -ryhmä. Yleiset järjestelmänvalvojat, ryhmän järjestelmänvalvojat, käyttäjätilien järjestelmänvalvojat, intune-palvelun järjestelmänvalvojat, kumppanitason1 tai tason 2 tuki sekä ryhmän omistaja voivat palauttaa ryhmän.
4. Kun dynaaminen ryhmä poistetaan ja palautetaan, se näkyy uudesta ryhmästä ja täytetään uudelleen säännön mukaan. Tämä prosessi voi kestää jopa 24 tuntia.
5. Lisätietoja poistetun ryhmän palauttamisesta on ohjeaiheessa [Poistetun Office 365 -ryhmän palauttaminen Azure Active Directoryssa.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)

**Ryhmän vanhenemiskäytännön määritys**

1. Tätä toimintoa tuetaan vain Office 365 -ryhmissä, ei käyttöoikeusryhmissä ja jakeluryhmissä.
2. Office 365 -ryhmien vanhenemiskäytännön määrittäminen ja käyttäminen edellyttää Azure AD Premium -käyttöoikeutta.
3. Tällä hetkellä vuokraajan Office 365 -ryhmille voidaan määrittää vain yksi vanhenemiskäytäntö.
4. Vain yleiset järjestelmänvalvojat, ryhmän järjestelmänvalvojat, käyttäjien järjestelmänvalvojat ja ryhmän omistaja voivat uusia ryhmän.
5. Jos Office 365 -ryhmä on vanhentunut, se poistetaan ja se voidaan palauttaa vain 30 päivää ennen pysyvää poistamista. Kun ryhmä on poistettu pysyvästi, sitä ei voi enää palauttaa. Lisätietoja ryhmien palauttamisesta [on täällä.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)

**Toimintopohjainen automaattinen uusiminen**

SharePointin, Outlookin ja Teamsin käyttäjien toiminnot voivat käynnistää ryhmän automaattisen uusimisen. Toiminnot tarkistetaan 35 päivän kuluttua ennen ryhmän vanhenemista. Jos ryhmän nykyisen elinkaaren aikana on toimintaa, ryhmä uusitaan automaattisesti eikä ryhmän omistajille lähetetä sähköposti-ilmoitusta.

**Vanhentuneiden ryhmien ilmoitusten ajoitus**

1. Sähköposti-ilmoitukset lähetetään Office 365 -ryhmien omistajille 30 päivää, 15 päivää ja 1 päivä ennen ryhmän vanhenemista.
2. Kun määrität vanhenemisen ensimmäisen kerran, vanhenemisväliä vanhemmat ryhmät määritetään 35 päivän kuluttua vanhenemiseen.
3. Ryhmän vanhentumispäivä lasketaan ryhmän uusimispäivän perusteella, ei päivitetyn käytännön mukaan. Jos vanhenemiskäytäntö päivitetään, vanhentumispäivä ei muutu.
4. Lisätietoja on kohdassa Ryhmän [vanhenemiskäytäntö ja uusiminen](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) sähköpostit sekä [poistetun Office 365 -ryhmän palauttaminen Azure Active Directoryssa.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)

**Ryhmän luontioikeus**

Varmista, että sinulla on oikeus luoda uusi ryhmä. Yleiset järjestelmänvalvojat voivat poistaa ryhmän luomisen käytöstä Azure-portaalissa tai -käyttöpaneelissa. Tarvitset ehkä järjestelmänvalvojan, jotta voit luoda uuden ryhmän, tai antaa sinulle tarvittavat käyttöoikeudet.

1. [Uuden ryhmän luominen ja jäsenten lisääminen Azure-portaalissa](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [Ryhmien luominen Powershell MSOnlinessa](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [Ryhmien luomisen poistaminen käytöstä PowerShellissä](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [Ryhmien luontien hallinta Office 365:ssä](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [Office 365:n tervetuloilmoituksen poistaminen käytöstä PowerShellin kautta](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [Azure AD:n järjestelmänvalvojan roolit](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**Ryhmän luontioikeuksien hallinta**

1. Yleiset järjestelmänvalvojat voivat hallita Azure-portaalissa tai -käyttöpaneelissa luotujen suojauksen tai  Office 365 -ryhmien ryhmän luontioikeuksia määrittämällä käyttäjät voivat luoda käyttöoikeusryhmiä Azure-portaaleissa tai käyttäjät voivat luoda **Office 365 -ryhmiä Azure-portaalin** asetuksissa Kaikissa ryhmissä **> Yleiset (Asetukset)**.
2. Voit myös rajoittaa ryhmän luomisen valitsemaan käyttäjäryhmän, jos sinulla on Azure AD P1 Premium -käyttöoikeus.

**Office 365 -ryhmän uusien jäsenten tervetuloilmoituksen poistaminen käytöstä**

Office 365 -ryhmiin lisätyille käyttäjille lähetetyn tervetuloilmoituksen voi poistaa käytöstä määrittämällä `UnifiedGroupWelcomeMessageEnabled` PowerShellissä  epätosi-asetuksen. Lisätietoja tästä [asetuksesta on täällä.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)













