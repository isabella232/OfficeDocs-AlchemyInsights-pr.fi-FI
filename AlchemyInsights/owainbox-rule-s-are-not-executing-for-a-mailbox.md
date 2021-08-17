---
title: 1332 OWA - Saapuneet-kansion sääntöjä ei suoriteta postilaatikolle
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
ms.openlocfilehash: b05ed9f0ee8c18b49b5338c53e67a79f1bf65464385dfa0ebd0639172a1b18f2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040899"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Saapuneet-kansion sääntö ei toimi odotetulla tavalla

Tarkista seuraavat asetukset Outlookin verkkoversio:

- Viestin voi ohjata uudelleen, lähettää edelleen tai vastata automaattisesti Saapuneet-kansion sääntöjen perusteella vain kerran. Uudelleenohjaussääntö (Saapuneet-kansion sääntö tai postinkulkusääntö eli siirtosääntö) voi lisätä viestiin enintään kymmenen vastaanottajaa. Lisätietoja on kohdassa [Päivyri-, Siirto- ja Saapuneet-kansion sääntörajoitukset.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)

- Saapuneet-kansion säännöt eivät toimi vaihtoehtoisessa päivyripostilaatikossa. Lisätietoja vaihtoehtoisesta päivyripostilaatikosta on kohdassa Vaihtoehtoinen [päivyripostilaatikko.](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)

Lisätietoja näiden ongelmien korjaamisesta on artikkelissa [KT-2829319.](https://support.microsoft.com/kb/2829319)

Jos edelliset ongelmat eivät päde, suorita Saapuneet-kansion säännön vianmääritysraportti, ennen kuin eskaloit ongelman Microsoft-tukeen:

1. Avaa postilaatikko Outlookin verkkoversio ja valitse <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Asetukset**  >  **Kaikkien Outlook Asetukset**  >  **Sähköposti**  >  **Säännöt**.

2. Valitse sivun alareunassa Jos säännöt **eivät toimi,** luo vianmääritysraportti napsauttamalla tätä .
