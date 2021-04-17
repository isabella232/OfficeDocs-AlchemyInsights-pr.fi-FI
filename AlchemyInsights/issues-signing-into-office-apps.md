---
title: Microsoft 365 -sovelluksiin kirjautumisongelmat
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833000"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Microsoft 365 -sovellusten "Tietokoneen Luotetut ympäristöt -moduuli ei toimi oikein" -viestin asentaminen

Voit korjata ongelman toimimalla seuraavasti:

- Asenna Windowsin ja Officen [uusimmat](https://support.microsoft.com/help/4027667/windows-10-update) [päivitykset.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Poista Office-tunnistetiedot](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) Windowsin tunnistetietojen hallinnan avulla.<br/>
    **Huomautus:** Office 2016:n rekisteripolut ovat muuttuneet 16.0-versioksi. (Esim: \Software\Microsoft\Office\16.0\Common\Identity\)
- Yritä korjata [TPM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) (Trusted Platform Module) -ongelmat käyttäjän palautusprosessin avulla.
- Määritä EnableADAL = 0 seuraavasti:  
    1. Napsauta Windowsin Käynnistä-painiketta hiiren kakkospainikkeella, **valitse Suorita**, **kirjoita regedit** ja valitse sitten **OK.**
    2. Salli **Rekisterieditorin** tehdä muutoksia laitteeseesi valitsemalla Kyllä.
    3. Lisää Rekisterieditorissa **EnableADAL:n DWORD-arvo,** jonka asetuksena on **0** kohdassa HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Lisätietoja on kohdassa Kirjautumisen yhteysongelmat [Windows 10:n Office 2016 -koontiversioon 16.0.7967 päivittämisen jälkeen.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)