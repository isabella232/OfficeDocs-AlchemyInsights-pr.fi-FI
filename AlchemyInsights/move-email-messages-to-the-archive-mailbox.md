---
title: Sähkö posti viestien siirtäminen arkiston posti laatikkoon
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822159"
---
# <a name="move-email-to-the-archive-mailbox"></a>Sähkö postin siirtäminen arkiston posti laatikkoon

1. Varmista, että **arkiston posti laatikko** on otettu käyttöön. Jos näin ei ole, ota Arkisto-posti laatikko käyttöön [tässä artikkelissa](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) olevien ohjeiden avulla.

2. Jos haluat arkistoida viestit automaattisesti Arkisto-posti laatikkoon, säilytys tunniste, jossa on **Siirrä arkistoon** -toiminto, täytyy määrittää **käyttöön automaattisesti koko posti laatikko (oletus)-tunnisteella**. Luo tagi: [Arkistoi oletus tunniste](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)tämän ohjeiden avulla.

3. Lisää seuraavaksi **Arkisto** tunniste säilytys käytäntöön. Valitse Exchangen hallinta keskuksessa **säilytys käytännöt** > Lisää **Siirrä arkistoon-tunnisteeseen** käytäntö > **Tallenna**.

4. [Määritä nyt säilytys käytäntö](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) tietyn käyttäjän posti laatikkoon. Sama käytäntö otetaan käyttöön sekä **ensisijaisessa** että **arkistossa** olevassa posti laatikossa.

Hallitun kansion apulainen (MFA) voi olla tarpeen pakottaa suorittamaan ja soveltamaan uusia asetuksia käyttäjän posti laatikkoon. Suorita seuraava komento ollessaan [yhteydessä EXO PowerShelliin](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) ja Käynnistä hallitun kansion avustaja tietyssä posti laatikossa:
  
Start-ManagedFolderAssistant-identiteetti<name of the mailbox>

Lisä tietoja arkistointi käytännön määrittämisestä on kohdassa [Posti laatikoiden arkistointi-ja poisto käytännön määrittäminen](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  