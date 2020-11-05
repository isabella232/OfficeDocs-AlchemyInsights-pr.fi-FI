---
title: Azure-laskutuksen omistajuuden siirtäminen
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
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922073"
---
# <a name="transfer-azure-billing-ownership"></a>Azure-laskutuksen omistajuuden siirtäminen

Kirjaudu sisään Azure- [portaaliin](https://portal.azure.com/) sen laskutus tilin järjestelmänvalvojana, jonka tila uksen haluat siirtää. Jos et ole varma, onko olet järjestelmänvalvoja tai jos haluat selvittää, kuka on, Katso lisä tietoja artikkelista [tilin laskutuksen hallinnoijan määrittäminen](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

- Etsi **kustannusten hallinta + laskutus**.
- Valitse **paketteja** vasemmasta ruudusta. Käyttö oikeuksien mukaan sinun on ehkä valittava laskutus alue ja sitten **tila uksia** tai **Azure-tila uksia**.
- Valitse Siirrä **laskutuksen omistajuus** tilaukselle, jonka haluat siirtää.
- Kirjoita sen käyttäjän Sähkö posti osoite, joka on sen tilin laskutuksen järjestelmänvalvoja, joka on uuden tila uksen omistaja ja valitse sitten **Lähetä siirto pyyntö**
- Käyttäjä saa Sähkö posti viestin, jossa on ohjeet siirto pyynnön tarkistamiseen. Jos haluat hyväksyä siirto pyynnön, käyttäjä valitsee Sähkö posti viestissä olevan linkin ja noudattaa annettuja ohjeita.

**Huomautus** : Jos siirrät tila uksen laskutuksen omistajuuden toisen Azure AD-vuokra ajan käyttäjän tiliin, Kaikki tila uksen resurssien hallintaan tarvittavat [Roolipohjaiset käyttö oikeuksien hallinta](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)tehtävät poistetaan pysyvästi. Vain uudella omistajalla on oikeus hallita tila uksen resursseja. Lisä tietoja on Ohje aiheessa [tila uksen siirtäminen käyttäjälle toisessa Azure AD-vuokra](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)ajassa.

**Suositellut asia kirjat**

- [Azure-tila uksen laskutuksen omistajuuden siirtäminen toiselle tilille](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Tietoja siitä, miten laskutus omistajuus siirretään Azure-tila ukseen](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Visual Studion, Microsoft-partneri verkoston (MPN) siirtäminen ja maksu tapa-ja kokeilu tilaukset](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Siirrä omistajuuden usein kysytyt kysymykset](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Siirron omistus ongelmien vian määritys](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
