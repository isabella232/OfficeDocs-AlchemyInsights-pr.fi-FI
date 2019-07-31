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
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938199"
---
# <a name="blank-sign-in-screen-in-office-apps"></a>Tyhjä kirjautumisnäytössä Office apps-

Voit korjata tämän ongelman, toimi seuraavasti:
- Asenna uusimmat päivitykset [Windows](https://support.microsoft.com/help/4027667/windows-10-update) ja [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Palauta Internet Explorerin asetukset: Siirry **Työkalut** > **Internet-asetukset** > **Advanced** > (Huomaa, että menetät mukautetut asetukset)**Palauta Internet Explorerin asetukset** ja yritä sitten kirjautua sisään Office uudelleen.
- Poista käytöstä Windows Defender sovelluksen Guard (WDAG) tai vastaava palomuuria tai virustentorjunta ohjelma:
    1. Ohjauspaneelin Siirry **Ohjelmat**ja valitse sitten **Windowsin ominaisuuksien ottaminen käyttöön tai poistaminen käytöstä**.
    2. Jos Windows Defender sovelluksen Guard on käytössä, poista se käytöstä.<br/>
    **Huomautus:** Saatat joutua käynnistämään tietokoneen uudelleen.
- Varmista, että Microsoft.AAD.BrokerPlugin [AAD WAM-laajennus](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ei ole estää minkä tahansa sovelluksen tai palomuuri tai vastaisten-virus ohjelma.
- [Poista Office-tunnistetietoja](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windowsin käyttöoikeuksien hallinnan.<br/>
    **Huomautus:** Office-2016 Rekisteripolut ovat muuttuneet 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Lisätietoja on kohdassa [yhteyden ongelmia sisään Office 2016 build 16.0.7967 10 Windows-päivityksen jälkeen](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).