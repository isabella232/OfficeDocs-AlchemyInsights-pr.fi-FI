---
title: Sähköpostiviestien siirtäminen Arkisto-postilaatikkoon
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
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974954"
---
# <a name="move-email-to-the-archive-mailbox"></a>Sähköpostin siirtäminen arkistopostilaatikkoon

Jos haluat, että suoritamme automaattiset tarkistukset alla mainittujen asetusten varalta, valitse Sivun ylä < -Takaisin-painike ja kirjoita sitten sen käyttäjän sähköpostiosoite, jolla on ongelmia sähköpostin siirtämisessä arkistopostilaatikkoon.

1. Varmista, että **arkistopostilaatikko** on otettu käyttöön. Jos näin ei ole, ota [arkistopostilaatikko](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) käyttöön tämän artikkelin ohjeiden mukaisesti.

2. Jos haluat arkistoida viestit automaattisesti arkistopostilaatikkoon, Siirrä arkistoon -toiminnon säilytystunniste on määritettävä automaattisesti käyttöön koko **postilaatikon (oletus) tunnisteessa.**  Luo tunniste noudattamalla tässä olevia ohjeita: [Arkistoi oletustunniste](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Lisää seuraavaksi **Arkisto-tunniste** säilytyskäytäntöösi. Valitse Exchange hallintakeskuksessa Säilytyskäytännöt ja **>** Siirrä **arkistoon -tunniste** käytännön > **Tallenna.**

4. Määritä [nyt säilytyskäytäntö](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) käyttäjän postilaatikkoon. Sama käytäntö otetaan käyttöön sekä ensisijaisessa **postilaatikossa** että **arkistopostilaatikossa.**

Voi olla tarpeen pakottaa Kansion hallinta -avustaja (MFA) toimimaan ja ottaa uudet asetukset käyttöön käyttäjän postilaatikossa. Käynnistä tietyn postilaatikon [hallittu kansioavustaja](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) suoritamalla seuraava komento, kun yhteys EXO PowerShelliin on muodostettu:
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

Lisätietoja arkistointikäytännön määrittämisestä on kohdassa [Postilaatikoiden arkistointi- ja poistokäytännön määrittäminen.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)
  