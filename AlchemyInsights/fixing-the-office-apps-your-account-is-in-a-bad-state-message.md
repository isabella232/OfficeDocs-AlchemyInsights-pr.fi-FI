---
title: Office-sovellusten korjaaminen Tilisi on huonossa tilassa -viesti
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969407"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>Office-sovellusten korjaaminen "Tilisi on huonossa tilassa" -virheen korjaaminen

Voit korjata tämän virheen kokeilemalla seuraavia asetuksia haavoittuvuuden sisältävässä tietokoneessa:

- Avaa Office-sovellus ja valitse **Kaikkien** > tilien**tiedostotilin** > **uloskirjautuminen**. Kirjaudu uudelleen sisään käyttäjätilillä, jolla on voimassa oleva käyttöoikeus. Lisätietoja on kohdassa [Office -tilit](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Tyhjennä Office-tunnistetiedot](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) WindowsIn tunnistetietojen hallinnan avulla.<br>
  **Huomautus:** Office 2016:n rekisteripolut ovat muuttuneet 16.0:ksi. Esimerkiksi \Software\Microsoft\Office\16.0\Common\Identity\
- Määritä haavoittuvuuden sisältävässä tietokoneessa EnableADAL = 0 seuraavasti:  
     1. Napsauta Windows-painiketta hiiren kakkospainikkeella ja valitse **Suorita**. Kirjoita **Avaa-ruutuun** **regedit**ja valitse sitten **OK**.
     2. Valitse **Kyllä,** kun näyttöön tulee kehote antaa Rekisterieditorin tehdä muutoksia laitteeseen.
    3. Lisää Rekisterieditorissa EnableADAL-arvo, jonka asetus on HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.
- Jos virhe ilmenee muodostettaessa yhteyttä Office 365:een Office 2013:n avulla, ota office-asiakasohjelman [moderni todennus käyttöön.](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)

Lisätietoja on [ohjeaiheessa Muiden kuin selainsovellusten vianmääritys, jotka eivät voi kirjautua Office 365:een, Azureen tai Intuneen.](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)

