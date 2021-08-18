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
- "2556"
ms.openlocfilehash: 7a8a0b68fc211e99b22e857d51d1de54e53a69357f75a0c60b1e83078cd5b27f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088033"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Tyhjä kirjautumisnäyttö Microsoft 365 sovelluksissa

Voit korjata ongelman kokeilemalla seuraavaa:
- Asenna uusimmat päivitykset [Windows](https://support.microsoft.com/help/4027667/windows-10-update) [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Palauta Internet Explorerin asetukset: Valitse Työkalut Internet-asetukset Internet  >    >    >  **Explorerin Asetukset asetusten** lisäasetukset (huomaa, että menetät mukautetut asetukset) ja yritä sitten kirjautua sisään Office uudelleen.
- Poista Windows Defenderin sovellussuoja (WDAG) tai muu vastaava palomuuri tai virustorjuntaohjelma käytöstä:
    1. Valitse Ohjauspaneelissa Ohjelmat ja **valitse sitten** Ota Windows käyttöön tai poista **se käytöstä**.
    2. Jos Windows Defenderin sovellussuoja on otettu käyttöön, kokeile poistaa se käytöstä.<br/>
    **Huomautus:** Tietokone on ehkä käynnistettävä uudelleen.
- Varmista, että jokin sovellus tai palomuuri tai virustorjuntaohjelma ei estä Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) -laajennusta.
- [Poista Office tunnistetiedot](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) tunnistetietojen Windows avulla.<br/>
    **Huomautus:** Office 2016:n rekisteripolut ovat muuttuneet 16.0-arvoksi. (Esim: \Software\Microsoft\Office\16.0\Common\Identity\)

Lisätietoja on ohjeaiheessa Kirjautumisongelmat kirjautumisen jälkeen Office [2016 -koontiversioon 16.0.7967 Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)