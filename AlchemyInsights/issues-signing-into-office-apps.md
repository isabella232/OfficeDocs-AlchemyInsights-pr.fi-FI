---
title: Ongelmia, jotka liittyvät Microsoft 365-sovelluksiin kirjautumiseen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695176"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Microsoft 365-sovellusten korjaaminen "tieto koneen luotettu käyttö ympäristö moduuli ei toimi oikein"-viesti

Voit korjata ongelman toimimalla seuraavasti:

- Asenna [Windowsin](https://support.microsoft.com/help/4027667/windows-10-update) ja [Officen](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)uusimmat päivitykset.
- [Poista Officen tunniste tiedot käyttämällä Windows Credential](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Manageria.<br/>
    **Huomautus:** Office 2016-rekisteri polut ovat muuttuneet 16,0-asetuksiksi. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Yritä korjata TPM (Trusted Platform Module)-vikoja kokeilemalla [Käyttäjän palautus prosessia](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) .
- Aseta EnableADAL = 0 seuraavien vaiheiden avulla:  
    1. Napsauta Windowsin Käynnistä-painiketta hiiren kakkos painikkeella, valitse **Suorita**, kirjoita **regedit**ja valitse sitten **OK**.
    2. Valitse **Kyllä** , jos haluat sallia rekisteri editorin tehdä muutoksia laitteeseesi.
    3. Lisää rekisteri editorissa **Enableadal:n** DWORD-arvo, jonka asetus on **0** , HKEY_CURRENT_USER \Ohjelmatiedostot\office\16.0\common\identty.

Lisä tietoja on kohdassa [kirjautumisen yhteys ongelmat sen jälkeen, kun olet päivittänyt Office 2016-koonti version 16.0.7967 Windows 10: ssä](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).