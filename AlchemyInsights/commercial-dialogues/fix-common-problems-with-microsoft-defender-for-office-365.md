---
title: Microsoft Defender for Windowsin yleisimmät Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: c5043bcd3d40dccc76b348f436001408e42ee7f9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330057"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>Microsoft Defender for Windowsin yleisimmät Office 365

Seuraavassa on joitakin ratkaisuja Microsoft Defender for Office 365 yleisiin ongelmiin:

- **Viestin viive:**

  Sähköpostin toimituksen viiveet voivat aiheuttaa Lokero viestien liitteiden tarkistuksen. Lisätietoja on kohdassa Lokero [käytäntöasetusten määrittäminen.](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings)

- **Virheellisten positiivisten tai negatiivisten tulosten raportoiminen:**

  Lisätietoja on kohdassa Viestien [ja tiedostojen raportoiminen Microsoftille.](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft)

- **Ota Lokero -suojaus käyttöön:**

  1. Siirry Microsoft 365 Defender -portaalissa kohtaan <https://security.microsoft.com/> **Sähköposti- &-&** \> **Käytännöt-Lokero** sääntöjen uhkien \>  \>  **käytännöt.**

     Jos haluat siirtyä suoraan **Lokero linkit -sivulle,** valitse <https://security.microsoft.com/safelinksv2> .

  2. Valitse **Lokero-sivulla** käytäntö napsauttamalla käytännön nimeä.
  3. Tee näyttöön tulevassa tiedot-pikaikkunassa jompikumpi seuraavista toimista:
     - Jos haluat lisätä uuden käytännön, valitse **+ Luo**. Ohjattu toiminto käynnistyy, jotta voit määrittää käytäntöasetukset.
     - Jos haluat muokata aiemmin luotua käytäntöä, valitse käytäntö napsauttamalla käytännön nimeä. Valitse näyttöön tulevassa tietojen **pikaikkunassa MuokkaaSuojauksen** **asetukset -osassa.**
  4. Määritä **Suojausasetukset-sivulla** seuraavat asetukset:
     - Ota käyttöön **Valitse toiminto tuntemattomille mahdollisesti vahingollisille URL-osoitteille viesteissä**.
     - Valitse **Käytä turvallisia linkkejä organisaation sisällä lähetetyissä viesteissä**.

  Lisätietoja on kohdassa [Linkkikäytäntöjen Lokero Microsoft Defender for Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies)
