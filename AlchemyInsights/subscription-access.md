---
title: Tilauskäyttö
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
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999237"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Kirjautuminen Azureen ei onnistu selaimen ongelmien vuoksi (selain jumii, pyörii, ei lataudu jne.)

Voi olla, että uloskaava saattaa vaikuttaa. Tarkista, onko olemassa jatkuvaa käyttökehää: [Azure Health Status](https://status.azure.com/status/history/).

Kirjaudu ulos kaikista aktiivisista Azure-istunnoista. Käynnistä selaimen yksityinen tai incognito-tila.

Voit myös yrittää päivittää selaimen, käyttää toista selainta ja poistaa välimuistin evästeet, jos yllä oleva ei toimi.

Lisätietoja: [Kirjautumisongelmien vianmääritys](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Tilausten käyttö ei onnistu**

Varmista [Azure-portaalissa,](https://portal.azure.com/)että oikea Azure-hakemisto on valittuna oikealla yläkulmassa käyttäen tiliä.

Varmista [Azure-tilikeskuksessa,](https://account.windowsazure.com/Subscriptions)että tilin järjestelmänvalvoja on tilin järjestelmänvalvoja.

Lisätietoja: [Tilausten vianmääritys](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Laskutushistoriaa ei voi käyttää**

Tilin järjestelmänvalvojan on varmistattava, että laskutustietoja käyttäjä on lisätty Azure Active Directoryyn vieraskäyttäjäksi: Uuden käyttäjän lisääminen [tai poistaminen.](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)

Käyttäjällä on oltava yleisen järjestelmänvalvojan rooli: [Roolin määrittäminen käyttäjille.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)

Kun tämä on julkaistu, käyttäjälle voidaan antaa laskutuskäyttötietoja RBAC-käytäntöjä käyttämällä: [Myönnä laskutuskäyttö.](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)

**Suositellut asiakirjat**

-   [Azure-tilauksen hallinta ei onnistu kirjautumalla sisään](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)