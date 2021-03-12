---
title: Salasanapohjaisen saumattoman kertakirjautumisen (SSO) ongelmien vianmääritys
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
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714766"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Salasanapohjaisen saumattoman kertakirjautumisen (SSO) ongelmien vianmääritys

Lisätietoja salasanapohjaisen kirjautumisen perustoiminnot on ohjeaiheessa Salasanapohjainen todentaminen [Azure Active Directoryn avulla.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)

**Salasanapohjaisen kirjautumisen määrittäminen**

1. [Salasanapohjaisen kertakirjautumisen määrittäminen](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) – Tässä artikkelissa on lisätietoja salasanapohjaisesta kertakirjautumisvaihtoehdosta. Jos lisäämässäsi sovelluksessa tarvitaan mukautettuja määrityksiä ja sinun on käytettävä salasanapohjaisia SSO-pohjaisia, tämä artikkeli on tarkoitettu sinulle.
2. [Määritä salasanapohjainen kertakirjaus on-prem-sovelluksia](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) varten – Sovelluksen välityspalvelin tukee useita kertakirjaustiloja. Salasanapohjainen kirjautuminen on tarkoitettu sovelluksille, jotka käyttävät todennusta käyttäjänimen ja salasanan yhdistelmää. Kun määrität sovellukselle salasanapohjaisen kirjautumisen, käyttäjien on kirjauduttava paikalliseen sovellukseen kerran. Tämän jälkeen Azure Active Directory tallentaa kirjautumistiedot ja antaa ne automaattisesti sovellukseen, kun käyttäjät voivat käyttää sitä etäyhteyden kautta.
    - Sovelluksen pitäisi olla jo julkaistu ja testattu sovelluksen välityspalvelimen avulla. Jos näin ei ole, noudata [Azure AD -sovelluksen](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) välityspalvelimen kautta julkaistavien sovellusten ohjeita ja jatka sitten salasanapohjaisen kirjautumisen määritystä esiasennettavalle sovellukselle.

Lisätietoja salasanapohjaisen kertakirjautumisen vianmäärityksestä on ohjeaiheessa [Salasanapohjaisen kertakirjautumisen vianmääritys Azure AD:ssä](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
