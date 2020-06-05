---
title: Microsoft 365 -sovelluksiin kirjautumiseen liittyvät ongelmat
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
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579862"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Microsoft 365 -sovellusten "Tietokoneen Trusted Platform module ei toimi oikein" -sanoman korjaaminen

Voit korjata ongelman toimimalla seuraavasti:

- Asenna uusimmat [Windows-](https://support.microsoft.com/help/4027667/windows-10-update) ja [Office-päivitykset](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Tyhjennä Officen tunnistetiedot](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windowsin tunnistetietojen hallinnan avulla.<br/>
    **Huomautus:** Office 2016:n rekisteripolut ovat muuttuneet 16.0:ksi. (Esimerkiksi \Software\Microsoft\Office\16.0\Common\Identity\)
- Yritä korjata Trusted Platform Module (TPM) -virheet [käyttäjän palautusprosessilla.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2)
- Aseta EnableADAL = 0 seuraavasti:  
    1. Napsauta Windowsin Käynnistä-painiketta hiiren kakkospainikkeella, valitse **Suorita**, kirjoita **regedit**ja valitse sitten **OK**.
    2. Valitse **Kyllä,** jos haluat, että Rekisterieditori voi tehdä muutoksia laitteeseesi.
    3. Lisää Rekisterieditorissa **EnableADAL-arvo,** jonka asetus on **0** kohdassa HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Lisätietoja on [ohjeaiheessa Yhteysongelmat kirjautumisessa Office 2016-koontiversion 16.0.7967 päivittämisen jälkeen Windows 10:ssä](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).