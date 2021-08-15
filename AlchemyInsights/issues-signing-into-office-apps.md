---
title: Ongelmia kirjautumisessa Microsoft 365 sovelluksiin
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
ms.openlocfilehash: b0789a54f48b2850c1dad8651a8209449c805784bea96799f05e67c4bc43fdb0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986888"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Tietokoneen Microsoft 365 ei toimi oikein -sanoman "Tietokoneen Luotetut ympäristöt -moduuli ei toimi" -viestin asentaminen

Voit korjata ongelman toimimalla seuraavasti:

- Asenna uusimmat päivitykset [Windows](https://support.microsoft.com/help/4027667/windows-10-update) [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Poista Office tunnistetiedot](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) tunnistetietojen Windows avulla.<br/>
    **Huomautus:** Office 2016:n rekisteripolut ovat muuttuneet 16.0-arvoksi. (Esim: \Software\Microsoft\Office\16.0\Common\Identity\)
- Yritä korjata [TPM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) (Trusted Platform Module) -ongelmat käyttäjän palautusprosessin avulla.
- Määritä EnableADAL = 0 seuraavasti:  
    1. Napsauta hiiren kakkospainikkeella Windows Käynnistä-painiketta, **valitse Suorita**, kirjoita **regedit** ja valitse sitten **OK**.
    2. Salli **Rekisterieditorin** tehdä muutoksia laitteeseesi valitsemalla Kyllä.
    3. Lisää Rekisterieditorissa **EnableADAL:n DWORD-arvo,** jonka asetuksena on **0** kohdassa HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Lisätietoja on ohjeaiheessa Kirjautumisongelmat kirjautumisen jälkeen Office [2016 -koontiversioon 16.0.7967 Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)