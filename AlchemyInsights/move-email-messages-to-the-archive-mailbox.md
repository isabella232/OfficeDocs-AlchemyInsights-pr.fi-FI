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
ms.openlocfilehash: 35c11f1bfb7c61b28a64f0128c29ddf7b4fce939
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511037"
---
# <a name="move-email-to-the-archive-mailbox"></a>Sähköpostin siirtäminen arkistopostilaatikkoon

1. Varmista, että **Arkisto-postilaatikko** on otettu käyttöön. Jos näin ei ole, ota arkistopostilaatikko käyttöön [tämän artikkelin](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) ohjeiden mukaisesti.

2. Jos haluat arkistoida viestit automaattisesti arkistopostilaatikkoon, **Siirrä arkistoon** -toiminnon säilytystunniste on määritettävä **käytettäväksi automaattisesti koko postilaatikon (oletus) tunnisteessa**. Luo tunniste seuraavasti: [Arkistoi oletustunniste](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Lisää seuraavaksi **Arkisto-tunniste** säilytyskäytäntöösi. Valitse Exchange-hallintakeskuksessa **Säilytyskäytännöt** > lisää **Siirrä arkistoon -tunniste** > **Tallenna**- > .

4. [Määritä nyt säilytyskäytäntö](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) tietyn käyttäjän postilaatikkoon. Samaa käytäntöä sovelletaan sekä **Ensisijainen-** että **Arkisto-postilaatikkoon.**

Hallittujen kansioiden hallinta (MFA) on ehkä pakotettava suorittamaan ja uusien asetusten käyttöönottamiseksi käyttäjän postilaatikossa. Käynnistä tietyn postilaatikon hallittu kansio-apuri suorittamalla seuraava komento, kun [se on yhteydessä EXO PowerShelliin:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)
  
Start-ManagedFolderAssistant -Käyttäjätiedot<name of the mailbox>

Lisätietoja arkistokäytännön määrittämisestä on [ohjeaiheessa Arkisto- ja poistokäytännön määrittäminen postilaatikoille](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  