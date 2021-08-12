---
title: Sovelluksen rekisteröinnin omistajan ongelmat
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
ms.openlocfilehash: cd7533f09ed8361e134b81979532cdebbf49971c54553a0172c7527f30e319bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951130"
---
# <a name="app-registration-owner-issues"></a>Sovelluksen rekisteröinnin omistajan ongelmat

Seuraavassa on menetelmiä, joilla voit lisätä principals-määritteet omistajiksi sovellusten rekisteröintiä varten:

- Azure AD:n PowerShell-moduulin käyttäminen –

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Viite: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Azure CLI :n käyttäminen - `az ad app owner add`

    Viite: [az ad -sovelluksen omistaja](https://docs.microsoft.com/cli/azure/ad/app/owner)
- MS-Graph -

    Viite: [Omistajan lisääminen – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Azure AD -portaalin käyttäminen – Siirry [portal.azure.com](https://portal.azure.com/) > Azure Active Directory > -sovelluksen rekisteröinti > Valitse sovellus > Omistajat > Lisää omistajia

**Etkö voi tarkastella sovellusta sovelluksen rekisteröinnin lavatta, vaikka olet sovelluksen omistaja?**

Sovelluksen omistaja ei ole järjestelmänvalvojarooli. Jos Rajoita [Azure AD -hallintaportaaliin](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) -asetus on käytössä, vain järjestelmänvalvoja voi tarkastella sovelluksia sovelluksen rekisteröintiportaalissa. Jotta omistaja voi tarkastella sovelluksia, poista tämä asetus käytöstä (Aseta asetukseksi EI) tai määritä omistajan järjestelmänvalvojan rooli vain tietylle sovellukselle. Tarvitset kuitenkin P2-Azure AD Premium ja käyttöoikeuksien [Privileged Identity Management.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)
