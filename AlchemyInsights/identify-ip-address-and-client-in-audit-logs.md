---
title: IP-osoitteen ja asiakkaan tunnistaminen valvontalokeissa
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 80b652eb65612093252dee226a19ec74bc035faa
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508913"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>IP-osoitteen ja asiakkaan tunnistaminen valvontalokeissa

Microsoft 365 -käyttäjän tai -järjestelmänvalvojan toimintaa vastaava IP-osoite näkyy valvontalokeissa. Myös asiakastiedot kirjataan lokiin. Tässä ovat vaiheet tällaisten tietojen tunnistamiseksi

1. Kirjaudu Microsoft [365 Security & Compliance Centeriin.](https://protection.office.com/)

2. Siirry **Haun**  >  **valvontalokin hakusivulle.**

   Jos olet kiinnostunut tietystä aktiviteetista, valitse se **Aktiviteetit-luettelosta.** Jos näin ei ole, kaikki aktiviteetit palautetaan valitulle käyttäjälle (oletusasetus).

   **Huomautus:** Tietyt toiminnot eivät ehkä ole käytettävissä **Aktiviteetit-valikossa.** Nämä valvontakohteet palautetaan kuitenkin, jos **Näytä kaikkien aktiviteettien tulokset** on valittuna (oletusasetus).

3. Määritä käyttäjänimi Käyttäjät-kentässä, valitse aktiviteetille sopiva päivämääräalue ja valitse sitten **Etsi**. **Users**

Tuloksissa näet kyseisen aktiviteetin IP-osoitteen tulosruudussa. Valitse valvontatietue, jos haluat nähdä yksityiskohtaiset tiedot **Tiedot-pikaikkunassa** (esimerkiksi Asiakas, Käyttäjä, joka suoritti toiminnon jne.).

Lisätietoja on [ohjeaiheessa Vaarantuneen tilin käyttämiseen käytettävän tietokoneen IP-osoitteen etsiminen](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
