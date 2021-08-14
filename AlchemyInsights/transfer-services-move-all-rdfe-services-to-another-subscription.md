---
title: Siirtopalvelut – Siirrä kaikki RDFE-palvelut toiseen tilaukseen
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
- "9004116"
- "7196"
ms.openlocfilehash: 89217922b8b51f2548f9fff53bf80364c0e897b1d9b34bfb7016f0b0f197cf17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940050"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Siirtopalvelut – Siirrä kaikki RDFE-palvelut toiseen tilaukseen

**Resurssien siirtäminen**

Azure-resurssit voidaan siirtää samaan tilaukseen joko toiseen Azure-tilaukseen tai resurssiryhmään Azure-portaalissa, Azure PowerShellissä, Azure CLI:ssä tai REST-ohjelmointirajapinnassa resurssien siirtoa varten.

Ennen kuin voit siirtää resursseja, katso lisätietoja:

- [Tarkistusluettelo ennen resurssien siirrämista](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Siirrettävät palvelut](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Siirron vahvistaminen](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Palvelujen siirto-ohjeet](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Voit siirtää olemassa olevia resursseja toiseen resurssiryhmään tai tilaukseen käyttämällä:

- [Azure-portaali](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST-ohjelmointirajapinta](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Opetusohjelma: [Azure-resurssien siirtäminen toiseen resurssiryhmään tai tilaukseen](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Azure Resource Managerin virheiden vianmääritys**

Alla olevassa artikkeleissa on tietoja joistakin yleisistä Azuren käyttöönottoon virheistä ja niiden ratkaisemiseen liittyviä tietoja. Jos et löydä käyttöönottovirheen virhekoodia, katso Lisätietoja on kohdassa [Etsi virhekoodi.](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code)

- [Käyttöönottovirheiden vianmääritys](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Azure-resurssien uuteen resurssiryhmään tai tilaukseen siirtämisen vianmääritys](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Huomaa, että jos haluat päivittää Azure-tilauksesi, kuten siirtymisen maksuttomasta maksuksi, sinun on muunnettava tilauksesi.

- Jos haluat päivittää maksuttoman kokeiluversion, katso maksuttoman kokeiluversion tai Microsoft Imagine Azure -tilauksen päivittäminen [Pay-As-You-Go -tilaukseksi.](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)
- Jos haluat muuttaa pay-as-you-go -tiliä, katso [Azure Pay-As-You-Go -tilauksen muuttaminen toiseen tarjoukseen.](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)

**Voit lisätä tai liittää Azure-tilauksen Azure Active Directory vuokraajaan:**

1. Kirjaudu sisään ja valitse tilaus, jota haluat käyttää Azure-portaalin [Tilaukset-sivulta.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)
2. Valitse **Vaihda hakemisto**.
3. Tarkista mahdolliset varoitukset ja valitse sitten **Muuta**.
4. Hakemistoa muutetaan tilaukselle, ja saat onnistumisviestin.
5. Siirry *uuteen* hakemistoon hakemiston vaihtajalla. Voi kestää jopa 10 minuuttia, ennen kuin kaikki näkyy oikein.

**Suositellut asiakirjat**

- [Azure-tilauksen omistajuuden siirtäminen](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Resurssien siirtäminen uuteen resurssiryhmään tai tilaukseen](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Resurssien hallinta Azure-portaalin avulla](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
