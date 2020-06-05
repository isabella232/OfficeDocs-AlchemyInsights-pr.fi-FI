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
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579898"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Tyhjä kirjautumisnäyttö Microsoft 365 -sovelluksissa

Voit korjata tämän ongelman kokeilemalla seuraavaa:
- Asenna uusimmat [Windows-](https://support.microsoft.com/help/4027667/windows-10-update) ja [Office-päivitykset](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Internet Explorerin asetusten palauttaminen: Siirry **Työkalut**  >  **Internet-asetukset**Internet  >  **Advanced**  >  **Explorerin asetusten lisäasetukset** -kohtaan (huomaa, että mukautetut asetukset menetetään) ja yritä sitten kirjautua uudelleen Officeen.
- Tehdä kykenemättömäksi Akkuna Puoltaa Ahkeruus Junailija (WDAG) eli jokin rinnakkainen polttopuut eli emission- myrkky ohjelmoida:
    1. Valitse Ohjauspaneelissa **Ohjelmat**ja valitse sitten **Ota Windowsin ominaisuudet käyttöön tai poista ne käytöstä**.
    2. Jos Windows Defender Application Guard on käytössä, kokeile poistaa se käytöstä.<br/>
    **Huomautus:** Tietokone on ehkä käynnistettävä uudelleen.
- Varmista, että mikään sovellus tai palomuuri/virustorjuntaohjelma ei estä Microsoft.AAD.BrokerPlugin [AAD WAM -laajennusta.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1)
- [Tyhjennä Officen tunnistetiedot](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windowsin tunnistetietojen hallinnan avulla.<br/>
    **Huomautus:** Office 2016:n rekisteripolut ovat muuttuneet 16.0:ksi. (Esimerkiksi \Software\Microsoft\Office\16.0\Common\Identity\)

Lisätietoja on [ohjeaiheessa Yhteysongelmat kirjautumisessa Office 2016-koontiversion 16.0.7967 päivittämisen jälkeen Windows 10:ssä](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).