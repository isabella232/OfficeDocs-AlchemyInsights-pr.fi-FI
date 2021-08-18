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
ms.openlocfilehash: f02daad7d4b4a11f8d8bb1ef1467db5809cbd291
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324359"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>Monitoimilaitteen tai sovelluksen määrittäminen lähettämään sähköpostia

Tietoja vaihtoehdoista ja toimintavaiheista on artikkelissa [Monitoimilaitteen tai sovelluksen määrittäminen lähettämään sähköpostia Microsoft 365:n avulla](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
Jos jokin laite tai sovellus lakkasi äskettäin toimimasta, yleisimmät ongelmat ovat seuraavat:

- **Todennukseen liittyvät virheet käytettäessä SMTP-todennusta asiakaslähetyksessä** Olemme hiljattain tehneet joitakin SMTP-todennuksen toimintaon liittyviä muutoksia. Lisätietoja ongelmien ratkaisemisesta on artikkelin Sähköpostin käyttäen sähköpostia sähköpostitse Microsoft 365 tai Office 365: todennus epäonnistui [-osassa.](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)
- **Hyväksymme vain TLS 1.2 -version, kun muodostamme suojatun yhteyden Office 365** Jos käytät suojattua yhteyttä (TLS), varmista, että sovelluslaite tukee TLS 1.2:ta. Lisätietoja on kohdassa [TLS 1.2:n](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)valmistelu Office 365 Office 365 GCC.
 
Lisätietoja muista ongelmista ja ratkaisuista on kohdassa Sähköpostin sähköpostisovelluksen kautta lähetettyjä tulostimia, skannereita ja lobsia Microsoft 365 [Office 365.](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)

Jos haluat nähdä, mistä laitteista on kyse, siirry [raporttiin SMTP-todennusta käyttävistä ohjelmista](https://protection.office.com/mailflow/dashboard).

**Huomautus:** Exchange Online ei mahdu joukkopostitusskenaarioihin. Jos haluat lähettää kaupallista joukkosähköpostia (esimerkiksi asiakkaan uutiskirjeitä), käytä näihin palveluihin erikoistamiasi kolmannen osapuolen palveluntarjoajia.
