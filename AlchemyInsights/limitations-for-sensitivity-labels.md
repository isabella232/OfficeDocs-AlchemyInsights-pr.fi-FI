---
title: Luottamuksellisuusotsikoiden rajoitukset Office tiedostoissa SharePoint OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: e197c43712c0ead9508a1cfdf48b51d01d2ae957649f73703f9c33733e332bf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813154"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>Luottamuksellisuusotsikoiden rajoitukset Office tiedostoissa SharePoint OneDrive

Kun otat käyttöön luottamuksellisuusotsikot Office tiedostoille SharePoint OneDrive, ota huomioon vaatimukset ja rajoitukset, jotka sisältävät seuraavat:

- SharePoint ja OneDrive eivät voi käsitellä joitakin Office-työpöytäsovelluksista merkittyjä ja salattuja tiedostoja, kun tiedostot sisältävät PowerQuery-tietoja, mukautettujen apuohjelmien tallentamia tietoja tai mukautettuja XML-osia.
- SharePoint ja OneDrive eivät lisää luottamuksellisuusotsikoita automaattisesti aiemmin salattuihin tiedostoihin Azure Information Protection (AIP) -selitteet. Luottamuksellisuusotsikoiden käyttö salatuissa tiedostoissa: 
    - Varmista, että AIP-selitteet on siirretty ja julkaistu Microsoft 365 yhteensopivuuskeskuksessa.
    - Lataa merkityt tiedostot ja lataa ne sitten alkuperäiseen SharePoint tai OneDrive sijaintiin.
- Jos tiedosto on salattu, tulostamista ei tueta.

Lisätietoja rajoituksista on kohdassa [Luottamuksellisuusotsikoiden ottaminen käyttöön Office tiedostoille SharePoint OneDrive.](/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations)
