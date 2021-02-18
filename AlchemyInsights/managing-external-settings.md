---
title: Ulkoisten asetusten hallinta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/17/2021
ms.locfileid: "50294212"
---
# <a name="managing-external-settings"></a>Ulkoisten asetusten hallinta

**Ilmoitus**

- [WebView-kirjautumistuen peruuttaminen Googlesta 4. tammikuuta 2021 alkaen.](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support) Testaa, vaikuttaako sovellustesi yhteensopivuus Googlen ohjeiden mukaisesti
- Varmista, että käytät järjestelmän verkkonäkymää tai järjestelmäselainta, kun kirjaudut sisään käyttäjiisi kuluttaja-Google-tileillä

**Kutsuasetusten hallinta**

Varmista, että olet [määrittänyt ulkoisen yhteistyön asetukset](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) niin, että asianmukaiset henkilöt voivat lähettää kutsuja.

**Vieraskäyttöoikeuksien hallinta**

1. Yleiset järjestelmänvalvojat voivat hallita hakemiston vieraskäyttöoikeuksia Azure-portaalin kautta määrittämällä vieraskäyttöoikeudet Ulkoisen yhteistyön asetukset -sivulla. [Lue lisää tästä asetusasetuksesta.](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support)
2. Jos haluat vieraiden voivan käyttää sovelluksia, kuten Teams tai SharePoint, varmista, että olet määrittänyt sovellukset sallimaan vieraskäyttö. Lisätietoja Teamsin [asetuksista ja](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) [SharePointista.](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support)

**Kutsujen määrittäminen:**

- [Ota B2B:n ulkoinen yhteistyö käyttöön ja hallitse sitä, ketkä voivat kutsua vieraita](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Tiettyjen organisaatioiden käyttäjien kutsujen salliminen tai estäminen](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

**Sallittujen tunnistetietojen palveluntarjoajien määrittäminen:**

- [Google Federation](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Suora liittouminen](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kertatunnistus sähköpostitse](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
