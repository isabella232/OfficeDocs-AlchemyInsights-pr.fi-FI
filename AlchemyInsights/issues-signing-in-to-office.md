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
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695284"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Microsoft 365-sovellusten tyhjä kirjautumisnäyttö

Voit korjata ongelman kokeilemalla seuraavaa:
- Asenna [Windowsin](https://support.microsoft.com/help/4027667/windows-10-update) ja [Officen](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)uusimmat päivitykset.
- Internet Explorerin asetusten palauttaminen: Valitse **Työkalut**-  >  kohdan**Internet-asetukset**  >  **Advanced**  >  **Palauta Internet Explorerin asetukset** (Huomaa, että menetät mukautetut asetukset) ja yritä kirja utua uudelleen sisään Officeen.
- Poista Windows Defender Application Guard (WDAG)-sovellus tai muu vastaava palo muuri tai virus torjunta ohjelma käytöstä:
    1. Valitse ohjaus paneelissa **ohjelmat**ja sitten **Ota Windowsin ominaisuudet käyttöön tai poista ne käytöstä**.
    2. Jos Windows Defender Application Guard on otettu käyttöön, poista se käytöstä.<br/>
    **Huomautus:** Sinun on ehkä käynnistettävä tieto kone uudelleen.
- Varmista, että jokin sovellus tai palo muuri/virus torjunta ohjelma ei estä Microsoft. AAD. BrokerPlugin AAD [WAM-laajennusta](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) .
- [Poista Officen tunniste tiedot käyttämällä Windows Credential](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Manageria.<br/>
    **Huomautus:** Office 2016-rekisteri polut ovat muuttuneet 16,0-asetuksiksi. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Lisä tietoja on kohdassa [kirjautumisen yhteys ongelmat sen jälkeen, kun olet päivittänyt Office 2016-koonti version 16.0.7967 Windows 10: ssä](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).