---
title: Azure-laskutuksen omistajuuden siirto
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
- "6849"
ms.openlocfilehash: 803d0105ad2bbaf2b18cea6aa556b6af5e09cb2d41812d4747aa703e6e7d7780
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036093"
---
# <a name="transfer-azure-billing-ownership"></a>Azure-laskutuksen omistajuuden siirto

Kirjaudu [Azure-portaaliin](https://portal.azure.com/) sen laskutustilin järjestelmänvalvojana, joka sisältää tilauksen, jonka haluat siirtää. Jos et ole varma, oletko järjestelmänvalvoja, tai jos haluat määrittää, kuka on, katso ohjeaihe [Määritä tilin laskutuksen järjestelmänvalvoja](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

1. Hae kohdasta _Kustannustenhallinta ja laskutus_.
1. Valitse **Tilaukset** vasemmasta ruudusta. Käyttöoikeuksista riippuen, sinun on ehkä valittava laskutuksen laajuus ja sitten **Tilaukset** tai **Azure-tilaukset**.
1. Valitse **Siirrä laskutuksen omistajuus** tilaukselle, jonka haluat siirtää.
1. Kirjoita sen käyttäjän sähköpostiosoite, joka on tilin laskutuksen järjestelmänvalvoja ja josta tehdään tilauksen uusi omistaja, ja valitse sitten **Lähetä siirtopyyntö**.
1. Käyttäjä saa sähköpostiviestin, jossa on ohjeet siirtopyyntösi tarkistamiseen. Käyttäjän on valittava sähköpostissa oleva linkki ja noudatettava annettuja ohjeita, jotta hän voi hyväksyä siirtopyynnön.

Huomaa, että jos siirrät tilauksesi laskutuksen omistajuuden toiselle Azure AD vuokralaiseen liittyvälle käyttäjälle, kaikki [roolipohjaiset käytönhallintatehtävät (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support), joiden avulla voit hallita tilauksesi resursseja, poistetaan pysyvästi. Vain uudella omistajalla on sen jälkeen oikeus hallita tilauksen resursseja. Lisätietoja tilauksen hakemiston muuttamisesta löytyy artikkelissa [Tilauksen siirtäminen käyttäjälle, joka kuuluu toiselle Azure AD -vuokralaiselle](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

_**Tärkeä vaikutus laskutukseesi:**_ Jos olet siirtänyt laskutuksen omistajuuden Azure -tilaukseen, sinulta tehtävät veloitukset ovat pro-rata-perusteisia. Voit käyttää laskuja seuraavasti:  

1. Valitse tilauksesi  [Tilaukset-sivulta](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Azure-portaalissa, [käyttäjänä, jolla on laskutuksen käyttöoikeudet](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support), ja valitse sitten **Laskut**.
1. Valitse **Lataa lasku** , jos haluat nähdä kopion PDF-laskusta. Jos siinä lukee _Ei saatavilla_, katso  [Miksi en näe laskua viimeiseltä laskutuskaudelta?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice).
1. Voit myös tarkastella päiväkohtaista käyttöäsi valitsemalla **laskutusjakson**, jolloin saat PDF-laskun ja yksityiskohtaisen tiedoston päiväkohtaisesta käytöstä (. CSV). Lisätietoja löytyy artikkelista  [Hae laskutus- ja käyttötiedot](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support).

**Suositellut asiakirjat**

- [Azure-tilauksen laskutuksen omistajuuden siirto toiselle tilille](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Tietoja laskutuksen omistajuuden Azure-tilauksen siirtämisestä](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Visual Studion, Microsoft-kumppaniverkoston (MPN) ja Maksa käytön mukaan -kehitys-/testitilauksiin](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Omistuksen siirtämiseen liittyvät usein kysytyt kysymykset](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Omistajuuden siirtoon liittyvien ongelmien vianmääritys](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
