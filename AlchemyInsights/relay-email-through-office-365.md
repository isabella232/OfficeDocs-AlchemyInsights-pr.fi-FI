---
title: Sähköpostin välittäminen Microsoft 365:n kautta
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: ef06cfe41eee5d67bf82d4f64875ddafac82ee2062aade761f81b906cd428dd5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024203"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>Monitoimilaitteen tai sovelluksen määrittäminen lähettämään sähköpostia

Tietoja vaihtoehdoista ja toimintavaiheista on artikkelissa [Monitoimilaitteen tai sovelluksen määrittäminen lähettämään sähköpostia Microsoft 365:n avulla](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
Jos jokin laite tai sovellus lakkasi äskettäin toimimasta, yleisimmät ongelmat ovat seuraavat:

- **Todennukseen liittyvät virheet käytettäessä SMTP-todennusta asiakaslähetyksessä** Olemme hiljattain tehneet joitakin SMTP-todennuksen toimintaon liittyviä muutoksia. Lisätietoja ongelmien ratkaisemisesta on artikkelin Sähköpostin käyttäen sähköpostia Microsoft 365 [](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)tai Office 365: todennus epäonnistui -osassa.
- **Hyväksymme vain TLS 1.2 -version, kun muodostamme suojatun yhteyden Office 365** Jos käytät suojattua yhteyttä (TLS), varmista, että sovelluslaite tukee TLS 1.2:ta. Lisätietoja on kohdassa [TLS 1.2:n](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)valmistelu Office 365 Office 365 GCC.
 
Lisätietoja muista ongelmista ja ratkaisuista on kohdassa Sähköpostin sähköpostisovelluksen kautta lähetetyissä tulostimiin, skanneri- ja lobriisisovelluksiin [Microsoft 365 tai Office 365.](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)

Jos haluat nähdä, mistä laitteista on kyse, siirry [raporttiin SMTP-todennusta käyttävistä ohjelmista](https://protection.office.com/mailflow/dashboard).

**Huomautus:** Exchange Online ei mahdu joukkopostitusskenaarioihin. Jos haluat lähettää kaupallista joukkosähköpostia (esimerkiksi asiakkaan uutiskirjeitä), käytä näihin palveluihin erikoistamiasi kolmannen osapuolen palveluntarjoajia.
