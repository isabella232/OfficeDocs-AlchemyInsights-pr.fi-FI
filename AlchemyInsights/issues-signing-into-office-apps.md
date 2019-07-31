---
title: Ongelmia Office-sovellusten kirjautua
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938200"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Vahvistettaessa Office apps ”tietokoneen Luotetut Platform module ei toimi kunnolla”-sanoma

Voit korjata tämän virheen, kokeile seuraavaa:

- Asenna uusimmat päivitykset [Windows](https://support.microsoft.com/help/4027667/windows-10-update) ja [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Poista Office-tunnistetietoja](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windowsin käyttöoikeuksien hallinnan.<br/>
    **Huomautus:** Office-2016 Rekisteripolut ovat muuttuneet 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Suorita [korjausohjelma käyttäjän](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) Trusted Platform Module (TPM) virheiden korjaamiseen.
- Määrittää EnableADAL = 0 seuraavasti:  
    1. Napsauta hiiren kakkospainikkeella Windowsin Käynnistä-painiketta, valitse **Suorita**, kirjoita **regedit**ja valitse sitten **OK**.
    2. Valitse **Kyllä** , jotta Registry Editor tehdä muutoksia laitteen.
    3. Registry Editor lisätä **EnableADAL** DWORD-arvon, joka on asetettu **0** HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity mukaisesti.

Lisätietoja on kohdassa [yhteyden ongelmia sisään Office 2016 build 16.0.7967 10 Windows-päivityksen jälkeen](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).