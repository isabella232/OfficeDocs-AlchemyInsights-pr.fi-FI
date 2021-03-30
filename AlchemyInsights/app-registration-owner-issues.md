---
title: Sovelluksen rekisteröintiomistajan ongelmat
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404456"
---
# <a name="app-registration-owner-issues"></a>Sovelluksen rekisteröintiomistajan ongelmat

Seuraavassa on menetelmät, joilla voit lisätä päätoimitsijat sovellusrekisteröinnit omistajiksi:

- Azure AD PowerShell -moduulin käyttäminen –

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Viite: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Azure CLI :n käyttäminen - `az ad app owner add`

    Viite: [az ad -sovelluksen omistaja](https://docs.microsoft.com/cli/azure/ad/app/owner)
- MS Graphin käyttäminen -

    Viite: [Omistajan lisääminen – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Azure AD -portaalin käyttäminen – Siirry [portal.azure.com](https://portal.azure.com/) > Azure Active Directoryyn > sovelluksen rekisteröintisovelluksen > Valitse > Omistajat > Lisää omistajia

**Etkö voi tarkastella sovellusta sovelluksen rekisteröintien lavatta, vaikka olet sovelluksen omistaja?**

Sovelluksen omistaja ei ole järjestelmänvalvojarooli. Jos Rajoita azure [AD -hallintaportaalin](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) käyttöä -asetus on käytössä, vain järjestelmänvalvoja voi tarkastella sovelluksia sovelluksen rekisteröintiportaalissa. Jotta omistaja voi tarkastella sovelluksia, joko poistaa tämän asetuksen käytöstä (Aseta asetukseksi EI) tai määrittää järjestelmänvalvojan roolin omistajalle vain tietyssä sovelluksessa. Tätä varten tarvitset kuitenkin Azure AD Premium P2 -käyttöoikeuden ja otat [Privileged Identity Managementin käyttöön.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)
