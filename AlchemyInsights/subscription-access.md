---
title: Tila uksen käyttäminen
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
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807431"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Kirjautuminen ei onnistu selaimen ongelmien vuoksi (selain jumittuu, pitää pyöriä, ei lataudu, jne.)

Sinulla voi olla katkos. Tarkista, onko käytössä jatkuva katkos: [Azure Health-tila](https://status.azure.com/status/history/).

Kirjaudu ulos kaikista Active Azure-istunnoista. Aloita selaimen yksityinen tai incognito-tila.

Voit myös yrittää päivittää selainta, käyttää toista selainta, poistaa väli muisti eväs teet, jos edellä ei toimi.

Lisä tietoja: [kirjautumisongelmien vian määritys](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Paketteja ei voi käyttää**

Varmista [Azure-portaalissa](https://portal.azure.com/), että oikea Azure-hakemisto on valittuna tilin oikeassa yläkulmassa.

Varmista [Azuren tili keskuksessa](https://account.windowsazure.com/Subscriptions), onko tili käytössä tilin järjestelmänvalvoja.

Lisä tietoja: [ei löydettyjä paketteja ei löydy](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Laskutus historiaa ei voi käyttää**

Tilin järjestelmänvalvojan on varmistettava, että laskutus tiedot sisältävä käyttäjä lisätään Azure Active Directoryyn vieras käyttäjänä: [uuden käyttäjän lisääminen tai poistaminen](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

Käyttäjälle on annettava yleinen järjestelmänvalvojan rooli: [roolin määrittäminen käyttäjille](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Lähetä tämä käyttäjä voi antaa laskutukseen pääsyn RBAC-käytäntöjen avulla: [Myönnä käyttö oikeudet laskutukseen](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Suositellut asia kirjat**

-   [En pysty Kirjautu maan Azure-tila uksen hallintaan](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)