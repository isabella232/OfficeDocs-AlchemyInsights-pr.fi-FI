---
title: Azure AD -todennuksen ja -valtuutuksen (AADSTS) virhekoodien vianmääritys
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036512"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>Azure AD -todennuksen ja -valtuutuksen (AADSTS) virhekoodien vianmääritys

Voit ratkaista AAD-todennuksen ja käyttöoikeuksien tarkistuksen virhekoodit (AADSTS) seuraavasti:

1. **Sovelluksen virhekoodien käsittely**

- **OAuth2.0-määritys** sisältää ohjeet virheiden käsittelemiseksi todennuksen https://tools.ietf.org/html/rfc6749#section-5.2 aikana virhevastauksen virheosan avulla.

    - **-virhe:** Virhekoodimerkkijono, jonka avulla voidaan luokitella ilmenevät virhetyypit ja jota tulee käyttää virheiden korjaamiseen.
    - **Virhekentässä** on useita mahdollisia arvoja: tutustu protokollan dokumentaatiolinkkeihin ja OAuth 2.0 :n tietoihin, niin saat lisätietoja virheistä ja niiden reagoinnista.

- Tässä on esimerkkivirhevastaus:
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **Haku nykyisen virhekoodin tiedot**

- Virhekoodit ja viestit voivat muuttua. Lisätietoja uusimmista tiedoista on sivulla, jossa on tietoja AADSTS-virheen kuvauksista, korjauksista ja joistakin ehdotetuista https://login.microsoftonline.com/error ratkaisuehdotuksista.
- Voit myös etsiä ja suorittaa vianmäärityksen [AADSTS-virhekoodeista,](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) jotka on lueteltu artikkelissa Azure AD -todennus- ja [valtuutusvirhekoodit.](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application)

3. **Hae ohjeita**

- [Tuki- ja ohjevaihtoehdot](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) kehittäjille – Jos tarvitset vastauksia ongelmaan, jota ei ole käsitelty asiakirjoissamme, sinun on ehkä aika ottaa yhteyttä asiantuntijoihin ja kysyä apua. Tässä artikkelissa on useita ehdotuksia kysymyksiin vastaamiseksi, kun kehität sovelluksia, jotka integroituvat Microsoftin tunnistetietoympäristöön.








