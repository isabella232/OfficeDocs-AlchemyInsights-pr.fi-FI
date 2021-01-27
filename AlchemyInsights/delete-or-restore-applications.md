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
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014799"
---
# <a name="delete-or-restore-applications"></a>Sovellusten poistaminen tai palauttaminen

**Sovelluksen poistaminen Azure AD -vuokraajassa:**

1. Valitse **Azure AD -portaalissa** **Yrityssovellukset.** Etsi ja valitse sitten sovellus, jonka haluat poistaa.
2. Valitse **vasemmanpuoleisen** ruudun Hallinta-osassa **Ominaisuudet.**
3. Vahvista **sovelluksen** poistaminen  Azure AD -vuokraajassa valitsemalla Poista ja valitsemalla sitten Kyllä.

Lisätietoja sovelluksen poistosta on pika-aloitustoiminn kohdassa: Sovelluksen poistaminen [Azure Active Directory (Azure AD) -vuokraajassa.](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

[PowerShellissä Remove-AzureADApplicationProxyApplication-cmdlet-komento](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) poistaa sovelluksen välityspalvelimen määritykset tietystä Azure Active Directoryn sovelluksesta ja voi poistaa sovelluksen kokonaan, jos se on määritetty.

Voit palauttaa **poistetun sovelluksen** PowerShellin avulla. Kun palautettava sovellus on tunnistettu, voit palauttaa sen [Restore-AzureADDeletedApplication-sovelluksella.](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
