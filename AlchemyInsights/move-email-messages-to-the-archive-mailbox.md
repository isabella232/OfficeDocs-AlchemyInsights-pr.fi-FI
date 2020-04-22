---
title: Sähköpostiviestien siirtäminen Arkisto-postilaatikkoon
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a5ad81e97df0ed5c337a622126173df94af80bb8
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713643"
---
# <a name="move-email-to-the-archive-mailbox"></a>Sähköpostin siirtäminen arkistopostilaatikkoon

1. Varmista, että **Arkisto-postilaatikko** on otettu käyttöön. Jos näin ei ole, ota arkistopostilaatikko käyttöön [tämän artikkelin](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) ohjeiden mukaisesti.

2. Jos haluat arkistoida viestit automaattisesti arkistopostilaatikkoon, säilytystunniste, jossa on **Siirrä arkistoon** -toiminto, on määritettävä **käytettäväksi automaattisesti koko postilaatikossa (oletus) -tunnisteessa.** Luo tunniste seuraavasti: [Arkistoi oletustunniste](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Lisää seuraavaksi **Arkisto-tunniste** säilytyskäytäntöön. Valitse Exchange-hallintakeskuksessa **Säilytyskäytännöt** > lisätä **Siirrä arkistoon -tunniste ->** **Tallenna**.

4. [Määritä säilytyskäytäntö](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) tietyn käyttäjän postilaatikkoon. Samaa käytäntöä sovelletaan sekä **Ensisijainen-** että **Arkisto-postilaatikkoon.**

Saattaa olla tarpeen pakottaa hallitun kansion avustaja (MFA) suorittamaan ja ottamaan uudet asetukset käyttöön käyttäjän postilaatikossa. Käynnistä tietyn postilaatikon hallitun kansion hallinta suorittamalla seuraava komento, kun [yhteys on muodostettu EXO PowerShelliin:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)
  
Start-ManagedFolderAssistant -Käyttäjätiedot<name of the mailbox>

Lisätietoja arkistokäytännön määrittämisestä on [ohjeaiheessa Postilaatikoiden arkisto- ja poistokäytännön määrittäminen](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  