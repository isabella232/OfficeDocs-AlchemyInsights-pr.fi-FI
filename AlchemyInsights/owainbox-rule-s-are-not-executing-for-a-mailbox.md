---
title: 1332 OWA-Saapuneet-kansion sääntöä ei voi suorittaa posti laatikolle
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f4d8db9c590abc490f193ef54a8a1dc5afba82b9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721588"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Saapuneet-kansion sääntö ei toimi oikein

Tarkista seuraavat asetukset Outlookin verkko versiossa:

- Viesti voidaan ohjata, lähettää edelleen tai vastata automaattisesti Saapuneet-kansion sääntöjen perusteella vain kerran. Uudelleenohjaus-sääntö (Saapuneet-kansion sääntö tai postin kulku sääntö, jota kutsutaan myös siirto säännöksi) voi lisätä viestiin enintään kymmenen edelleenlähetystä. Lisä tietoja on kohdassa [Päivyri-, siirto-ja Saapuneet-kansion sääntö rajat](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Saapuneet-kansion säännöt eivät toimi vaihtoehtoisessa lokiin kirjaamisen posti laatikossa. Lisä tietoja vaihtoehtoisesta lokiin kirjaamisen posti laatikosta on kohdassa [Vaihtoehtoinen lokiin kirjaaminen-posti laatikko](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Lisä tietoja ongelmien korjaamisesta on kohdassa [KB 2829319](https://support.microsoft.com/kb/2829319).

Jos edelliset ongelmat eivät ole voimassa, suorita Saapuneet-kansion säännön diagnostiikka raportti, ennen kuin eskaloit ongelman Microsoft-tukeen:

1. Avaa posti laatikko Outlookin verkko versiossa ja valitse <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Asetukset**  >  **Näytä kaikki Outlook-asetukset**  >  **Sähkö posti viesti**  >  **Säännöt**.

2. Napsauta sivun alaosassa, **Jos säännöt eivät toimi, luo diagnostiikka raportti napsauttamalla tätä**.
