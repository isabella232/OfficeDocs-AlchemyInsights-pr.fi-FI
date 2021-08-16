---
title: Tuetut tilaustyypit
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6675"
ms.openlocfilehash: f11eabdc18f708e34a6a10c67bc3e7416330cbf34aec20209b42252ffa0ab018
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072157"
---
# <a name="supported-subscription-types"></a>Tuetut tilaustyypit

Tarkista tuetut tilaustyypit, jotta voit jatkaa eteenpäin.

[Tuetut tilaustyypit](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Laskutuksen omistajuuden siirto**

Azure-portaaliin sen laskutustilin [järjestelmänvalvojana](https://ms.portal.azure.com/), jonka tilauksen haluat siirtää.

- Hae kohdasta **Kustannustenhallinta ja laskutus**. Valitse **Tilaukset** vasemmasta ruudusta. Käyttöoikeuksista riippuen, sinun on ehkä valittava laskutuksen laajuus ja sitten **Tilaukset** tai **Azure-tilaukset**.
- Valitse Siirrä laskutuksen omistajuus tilaukselle, jonka haluat siirtää.
- Kirjoita sen käyttäjän sähköpostiosoite, joka on tilin laskutuksen järjestelmänvalvoja ja josta tehdään tilauksen uusi omistaja, ja valitse sitten **Lähetä siirtopyyntö**.
- Käyttäjä saa sähköpostiviestin, jossa on ohjeet siirtopyyntösi tarkistamiseen. Käyttäjän on valittava sähköpostissa oleva linkki ja noudatettava annettuja ohjeita, jotta hän voi hyväksyä siirtopyynnön.

Huomaa, että jos siirrät tilauksesi laskutuksen omistajuuden toiselle Azure AD vuokralaiseen liittyvälle käyttäjälle, kaikki [roolipohjaiset käytönhallintatehtävät (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support), joiden avulla voit hallita tilauksesi resursseja, poistetaan pysyvästi. Vain uudella omistajalla on sen jälkeen oikeus hallita tilauksen resursseja. Lisätietoja tilauksen hakemiston muuttamisesta löytyy artikkelissa [Tilauksen siirtäminen käyttäjälle, joka kuuluu toiselle Azure AD -vuokralaiselle](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Tilauksen omistajuuden siirto**

Tilauksen omistajuuden siirron edellytykset ovat roolipohjainen käyttöoikeus (RBAC), jotta tilauksen resurssien hallinta ei menetä käyttöoikeuttaan. Lisätietoja olemassa olevan tilauksen lisäämisestä vuokraajaan on kohdassa [Azure-tilauksen liittäminen tai lisääminen Azure Active Directoryyn](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Tilauksen siirtoa, jonka nykyinen laskutusjakso sisältää olemassa olevan avoimen summan, ei siirretä uuden tilin uuteen maksuvälineeseen. Ainoa uuden tilin käyttäjien käytettävissä olevat tiedot ovat viime kuukauden tilauskustannukset. Muut käyttö- ja laskutushistorian tiedot eivät siirry tilaukseen.
- Enterprise Agreement (EA) -tilausten laskutuksen omistajuuden siirtoa tuetaan tällä hetkellä vain Enterprise Agreement -portaalissa
- Luottotietoisen tilauksen, kuten Visual Studion, BizSparkin ja Microsoft-kumppaniverkoston siirtäminen uudelle käyttäjälle edellyttää Visual Studio- tai Microsoft-kumppaniverkoston käyttöoikeutta siirtopyynnön hyväksymiseen.
- Kaikki resurssit, kuten virtuaalikoneet, levyt ja sivustot, siirretään onnistuneesti uuteen tiliin. Eri vuokraajatilausten siirrossa saattaa olla vaikutusta seuraaviin resursseihin:

**Azure AD -toimialuepalvelut**

Azure-avainsijainnit

- [Käyttäjiin ja tietokantoihin liittyvä SQL](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) voi vaikuttaa erityisesti, jos asiakas käyttää Azure Active Directoryyn liittyvää todennusta
- Saattaa vaikuttaa **Sovelluspalveluihin**, jotka on määritetty Azure Active Directory -todennuksella
- **Visual Studio Team** Services -tilit, jotka on yhdistetty Azure-tilauksia varten, voivat tilapäisesti menettää käyttöoikeuden, kun yhdistetty Azure-tilaus peruutetaan

**Suositellut asiakirjat**

Vaiheet laskutuksen omistajuuden hyväksymisen jälkeen:

- Jos haluat säilyttää laskutuksen omistajuuden, mutta muuttaa tilauksen tyyppiä, katso lisätietoja kohdasta [Azure-tilauksen vaihtaminen toiseen tarjoukseen](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Visual Studion, Microsoft-kumppaniverkoston (MPN) ja Maksa käytön mukaan -kehitys-/testitilauksiin](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Enterprise Agreement (EA) -tilausten laskutuksen omistajuuden siirtäminen](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Omistuksen siirtämiseen liittyvät usein kysytyt kysymykset](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Omistajuuden siirtoon liittyvien ongelmien vianmääritys](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)