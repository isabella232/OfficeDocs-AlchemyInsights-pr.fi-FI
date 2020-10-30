---
title: Tuetuissa tilaus tyypeissä
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6675"
ms.openlocfilehash: 46bc60435c3f8477e9f274d90c39d0f1c6a523c6
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807561"
---
# <a name="supported-subscription-types"></a>Tuetuissa tilaus tyypeissä

Tutustu tuetuissa tilaus tyypeissä jatkaaksesi.

[Tuetuissa tilaus tyypeissä](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Siirrä laskutuksen omistajuus**

Azure-portaali sen laskutus tilin [tilin](https://ms.portal.azure.com/) järjestelmänvalvojana, joka sisältää tila uksen, jonka haluat siirtää.

- Etsi **kustannusten hallinta + laskutus** . Valitse **paketteja** vasemmasta ruudusta. Käyttö oikeuksien mukaan sinun on ehkä valittava laskutus alue ja sitten **tila uksia** tai **Azure-tila uksia** .
- Valitse Siirrä laskutuksen omistajuus tilaukselle, jonka haluat siirtää.
- Kirjoita sen käyttäjän Sähkö posti osoite, joka on sen tilin laskutuksen järjestelmänvalvoja, joka on uuden tila uksen omistaja ja valitse sitten **Lähetä siirto pyyntö**
- Käyttäjä saa Sähkö posti viestin, jossa on ohjeet siirto pyynnön tarkistamiseen. Jos haluat hyväksyä siirto pyynnön, käyttäjä valitsee Sähkö posti viestissä olevan linkin ja noudattaa annettuja ohjeita.

Huomautus: Jos siirrät tila uksen laskutuksen omistajuuden toisen Azure AD-vuokra ajan käyttäjän tiliin, Kaikki tila uksen resurssien hallintaan tarvittavat [Roolipohjaiset käyttö oikeuksien hallinta](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) tehtävät poistetaan pysyvästi. Vain uudella omistajalla on oikeus hallita tila uksen resursseja. Lisä tietoja on Ohje aiheessa [tila uksen siirtäminen käyttäjälle toisessa Azure AD-vuokra](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)ajassa.

**Tila uksen omistajuuden siirtäminen**

Tilaus omistuksen siirto edellytykset roolipohjainen käyttöoikeus (RBAC), jolla hallitaan tila uksen resursseja, menettävät niiden käytön. Lisä tietoja olemassa olevan tila uksen lisäämisestä vuokraajaan on kohdassa Azure- [tila uksen liittäminen tai lisääminen Azure Active Directoryyn](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Tila uksen siirtoa, jossa nykyinen laskutus sykli sisältää nykyisen jäljellä olevan summan, ei siirretä uuden tilin uuteen maksu välineeseen. Vain uuden tilin käyttäjien käytettävissä olevat tiedot ovat tilauksesi viimeisen kuukauden kustannukset. Muu käyttö-ja laskutus historia ei siirry tila ukseen.
- Enterprise Agreement (EA)-tila uksien laskutusomistusta tuetaan tällä hetkellä vain Enterprise Agreement-portaalissa
- Jos haluat siirtää luotto tieto paketin, kuten Visual Studion, BizSpark, Microsoft-kumppanien verkoston, uudelle käyttäjälle edellyttää, että sinulla on Visual Studio/Microsoft-partneri verkoston käyttö oikeus, jotta voit hyväksyä siirto pyynnön
- Kaikki resurssit, kuten virtuaalikoneet, levykkeet ja sivustot, siirtyvät uudelle tilille. Seuraavat resurssit voivat vaikuttaa vuokra ajan tila uksen siirtoon:

**Azure AD-toimi alue palvelut**

Azure-avaimen varastojen

- [SQL-käyttäjät ja-tieto kannat](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) saattavat heikentyä, etenkin jos asiakas käyttää Azure Active Directoryyn liittyvää todennusta
- Azure Active Directory-todennukseen määritetyt **sovellus Palvelut** saattavat vaikuttaa
- **Visual Studio-tiimi** Azure-tila uksiin liitetyt palvelu asiakkaat voivat tilapäisesti menettää käytön, kun yhdistetty Azure-tilaus peruutetaan

**Suositellut asia kirjat**

Vaiheet sen jälkeen, kun olet hyväksynyt laskutuksen omistajuuden:

- Jos haluat säilyttää laskutuksen omistajuuden, mutta muuttaa tilauksesi tyyppiä, Katso lisä tieto: [Azure-tila uksen vaihtaminen toiseen tarjoukseen](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Visual Studion, Microsoft-partneri verkoston (MPN) siirtäminen ja maksu tapa-ja kokeilu tilaukset](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Siirrä Enterprise Agreement (EA)-tila uksen laskutuksen omistajuus](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Siirrä omistajuuden usein kysytyt kysymykset](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Siirron omistus ongelmien vian määritys](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)