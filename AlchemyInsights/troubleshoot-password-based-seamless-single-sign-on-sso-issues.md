---
title: Salasanapohjaisen saumattoman kertakirjautumisen ongelmien vianmääritys
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
ms.openlocfilehash: 6b4d7335461c913a6b5f782756684c5526a96c58c44853ddf9154aa51607bd4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972821"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Salasanapohjaisen saumattoman kertakirjautumisen ongelmien vianmääritys

Lisätietoja salasanapohjaisen SSO-kirjautumisen perussyistä on kohdassa Salasanapohjainen [todennus Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)

**Salasanapohjaisen SSO:n määrittäminen**

1. [Salasanapohjaisen kertakirjautumisen määrittäminen](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) – Tässä artikkelissa on lisätietoja salasanapohjaisesta kertakirjautumisvaihtoehdosta. Jos sovellus, jonka lisäät, vaatii mukautettuja määrityksiä ja sinun on käytettävä salasanaan perustuvaa SSO:ta, tämä artikkeli on tarkoitettu sinulle.
2. [Määritä salasanapohjainen kertakirjaus on-prem-sovelluksissa](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) – Sovelluksen välityspalvelin tukee useita kertakirjaustiloja. Salasanapohjainen kirjautuminen on tarkoitettu sovelluksille, jotka käyttävät todennusta käyttäjänimen ja salasanan yhdistelmää. Kun määrität sovellukselle salasanapohjaisen kirjautumisen, käyttäjien on kirjauduttava paikalliseen sovellukseen kerran. Sen jälkeen Azure Active Directory kirjautumistiedot ja antaa ne automaattisesti sovellukselle, kun käyttäjät voivat käyttää sitä etäyhteyden kautta.
    - Sinun pitäisi jo julkaista ja testata sovellus sovellusvälityspalvelimen avulla. Jos näin ei ole, noudata ohjeita, jotka ovat kohdan Sovellusten julkaiseminen [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) -sovellusvälityspalvelimen avulla, ja jatka sitten salasanapohjaisen kirjautumisen määritystä esiasennettavalle sovellukselle.

Lisätietoja salasanapohjaisen kertakirjautumisen vianmäärityksestä on kohdassa [Salasanapohjaisen kertakirjautumisen vianmääritys Azure AD:ssä](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
