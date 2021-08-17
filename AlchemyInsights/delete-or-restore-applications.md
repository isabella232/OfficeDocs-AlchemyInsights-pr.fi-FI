---
title: Sovellusten poistaminen tai palauttaminen
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
- "9004335"
- "7737"
ms.openlocfilehash: 0c7be98650ca87f36b66f0bb38fb665fc81525b7f3410da14b99fb67468c1e73
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102568"
---
# <a name="delete-or-restore-applications"></a>Sovellusten poistaminen tai palauttaminen

**Sovelluksen poistaminen Azure AD -vuokraajassa:**

1. Valitse **Azure AD -portaalissa** **Yrityssovellukset**. Etsi ja valitse sovellus, jonka haluat poistaa.
2. Valitse **vasemmanpuoleisen** ruudun Hallinta-osassa **Ominaisuudet**.
3. Valitse **Poista** ja vahvista **sitten,** että haluat poistaa sovelluksen Azure AD -vuokraajassa valitsemalla Kyllä.

Lisätietoja sovelluksen poistosta on kohdassa Pika-aloitustoiminto: Sovelluksen poistaminen [Azure Active Directory (Azure AD) -vuokraajassa.](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

PowerShellin [Remove-AzureADApplicationProxyApplication-cmdlet-komento](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) poistaa sovelluksen välityspalvelimen määritykset tietystä Azure Active Directory:ssä ja voi poistaa sovelluksen kokonaan, jos se on määritetty.

Voit palauttaa **poistetun sovelluksen** PowerShellin avulla. Kun palautettava sovellus on tunnistettu, voit palauttaa sen [Restore-AzureADDeletedApplication-sovelluksella.](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
