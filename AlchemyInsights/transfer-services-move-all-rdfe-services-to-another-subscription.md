---
title: Siirto Palvelut – Siirrä kaikki RFE-Palvelut toiseen tila ukseen
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
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692042"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Siirto Palvelut – Siirrä kaikki RFE-Palvelut toiseen tila ukseen

**Siirrä resursseja**

Azure-resurssit voidaan siirtää toiseen Azure-tila ukseen tai resurssi ryhmään saman tila uksen kautta käyttämällä Azure portaalia, Azure PowerShelliä, Azure CLI-liittymää tai REST-ohjelmointi raja pintaa resurssien siirtämiseen.

Ennen kuin voit siirtää resursseja, Katso:

- [Tarkistus luettelo ennen resurssien siirtämistä](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Siirrettävät palvelut](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Siirron vahvistaminen](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Palveluiden ohjeiden siirtäminen](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Jos haluat siirtää olemassa olevat resurssit toiseen resurssi ryhmään tai-tila ukseen, voit käyttää:

- [Azure-portaali](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST-OHJELMOINTI RAJA PINTA](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Opetus ohjelma: [Azure-resurssien siirtäminen toiseen resurssi ryhmään tai-tila ukseen](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Virheiden vian määritys Azure Resource Managerilla**

Seuraavissa artikkeleissa on lisä tietoja joistakin yleisistä Azure-käyttöönotto virheistä ja niiden ratkaisemisesta. Jos et löydä käyttöönotto virheesi virhe koodia, Katso lisä tietoja artikkelista [Virhe koodin](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code)hakeminen.

- [Käyttöönotto virheiden vian määritys](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Azure-resurssien siirtämiseen uuteen resurssi ryhmään tai-tila ukseen liittyviä ongelmia](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Huomaa, että jos haluat päivittää Azure-pakettisi, kuten siirtymisestä maksuttomien maksu tietojen mukaan, sinun on muunnettava pakettisi.

- Jos haluat päivittää maksuttomat kokeilu versiot, Katso lisä tietoja artikkelista [maksuttomien kokeilu versioiden päivittäminen tai Microsoft Imagine Azure-tilaus](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- Jos haluat muuttaa pay-as-you-go-tiliä, Katso lisä tietoja artikkelista [Azure pay-as-you-go-tila uksen vaihtaminen eri tarjoukseen](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).

**Azure-tila uksen lisääminen tai liittäminen Azure Active Directory-vuokraajaan:**

1. Kirjaudu sisään ja valitse tilaus, jota haluat käyttää [Azure-portaalin tila ukset-sivulla](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. Valitse **Vaihda hakemisto**.
3. Tarkista näkyviin tulevat varoitukset ja valitse sitten **Muuta**.
4. Tila uksen hakemistoa muutetaan ja saat Onnistumis viestin.
5. Siirry uuteen hakemistoon *hakemiston* valitsimen avulla. Voi kestää jopa 10 minuuttia, ennen kuin kaikki näkyy oikein.

**Suositellut asia kirjat**

- [Azure-tila uksen omistajuuden siirtäminen](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Resurssien siirtäminen uuteen resurssi ryhmään tai-tila ukseen](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Resurssien hallinta Azure-portaalin avulla](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
