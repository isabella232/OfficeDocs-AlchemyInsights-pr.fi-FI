---
title: Office-sovellusten korjaaminen Office-käyttöoikeuksien etsiminen ei ollut viesti
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 565df0a05baa974a6cbac58ac6be8d78470dbc5d
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715629"
---
# <a name="fixing-the-office-apps-couldnt-find-office-licenses-associated-message"></a>Office-sovellusten "Office-käyttöoikeuksia ei löydy" -sanoman korjaaminen

Jos saat tämän sanoman, kokeile seuraavaa:

1. Tarkista palomuurin, virustentorjuntaohjelmiston ja välityspalvelimen asetukset ja varmista, että ne eivät estä Office-sovellusten Internet-yhteyttä. Lisätietoja [on ohjeaiheessa Microsoft 365:n URL-osoitteet ja IP-osoitealueet](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Poista kyseisen käyttäjän [Office-käyttöoikeus](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) ja määritä se uudelleen. 
3. Avaa Office-sovellus ja [kirjaudu ulos](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) olemassa olevista käyttäjätileistä.
4. Siirry Windowsin asetukset -> **Tilit** > **Sähköposti & -tileille**ja poista kaikki työtilit, joita ei voi käyttää, paitsi kyseinen tili.
5. Siirry Windowsin asetukset -kohtaan > **Accounts** > **Accessin työ- tai koulukäyttöön**ja katkaise yhteys kaikkiin työtileihin paitsi tilin, jota asia koskee.
6. Palauta Officen aktivointitila. [Ohjeet](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Kirjaudu sisään](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) käyttämällä haavoittuvuuden sisältävää käyttäjätiliä.

Lisätietoja vianmääritysratkaisuista on artikkelissa [Käyttöoikeudettomat tuote- ja aktivointivirheet Officessa](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).