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
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833028"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Tyhjä kirjautumisnäyttö Microsoft 365 -sovelluksissa

Voit korjata ongelman kokeilemalla seuraavaa:
- Asenna Windowsin ja Officen [uusimmat](https://support.microsoft.com/help/4027667/windows-10-update) [päivitykset.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Palauta Internet Explorerin asetukset: Siirry **kohtaan Työkalut** Internet-asetusten palauttamisen lisäasetukset Internet Explorerin asetuksissa (huomaa, että menetät mukautetut asetukset) ja yritä sitten  >    >    >   kirjautua Officeen uudelleen.
- Poista Windows Defenderin sovellussuoja (WDAG) tai muu vastaava palomuuri tai virustorjuntaohjelma käytöstä:
    1. Valitse Ohjauspaneelissa Ohjelmat ja **valitse** sitten Ota **Windowsin ominaisuudet käyttöön tai poista ne käytöstä.**
    2. Jos Windows Defenderin sovellussuoja on käytössä, kokeile poistaa se käytöstä.<br/>
    **Huomautus:** Tietokone on ehkä käynnistettävä uudelleen.
- Varmista, että jokin sovellus tai palomuuri tai virustorjuntaohjelma ei estä Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) -laajennusta.
- [Poista Office-tunnistetiedot](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windowsin tunnistetietojen hallinnan avulla.<br/>
    **Huomautus:** Office 2016:n rekisteripolut ovat muuttuneet 16.0-versioksi. (Esim: \Software\Microsoft\Office\16.0\Common\Identity\)

Lisätietoja on kohdassa Kirjautumisen yhteysongelmat [Windows 10:n Office 2016 -koontiversioon 16.0.7967 päivittämisen jälkeen.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)