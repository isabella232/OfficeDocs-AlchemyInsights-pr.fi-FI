---
title: Microsoft 365 -sovelluksiin kirjautumisongelmat
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
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709103"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Tietokoneen luotetun ympäristön moduulin toimimattoman Microsoft 365 -sovellusten korjaamisen sanoma

Voit korjata ongelman toimimalla seuraavasti:

- Asenna Windowsin ja Officen [uusimmat](https://support.microsoft.com/help/4027667/windows-10-update) [päivitykset.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Poista Office-tunnistetiedot](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) Windowsin tunnistetietojen hallinnan avulla.<br/>
    **Huomautus:** Office 2016:n rekisteripolut ovat muuttuneet versioksi 16.0. (Esim: \Software\Microsoft\Office\16.0\Common\Identity\)
- Yritä käyttäjän [palautusprosessia luotettujen](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) ympäristömoduulien (TPM) ongelmien korjaamiseksi.
- Määritä EnableADAL = 0 seuraavasti:  
    1. Napsauta Windowsin Käynnistä-painiketta hiiren kakkospainikkeella, **valitse Suorita,** kirjoita **regedit** ja valitse **sitten OK.**
    2. Salli **Rekisterieditorin** tehdä muutoksia laitteeseen valitsemalla Kyllä.
    3. Lisää Rekisterieditorissa **EnableADAL-DWORD-arvo,** jonka asetuksena on **0,** HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Lisätietoja on kohdassa Kirjautumisongelmat kirjautumisen jälkeen, kun [Windows 10:n Office 2016 -koontiversioon 16.0.7967 on päivitetty.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)