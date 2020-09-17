---
title: Ehdollinen käyttäminen Intunella
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807656"
---
# <a name="conditional-access-with-intune"></a>Ehdollinen käyttäminen Intunella

**Ehdollisen käyttö oikeuden** käyttäminen Intunella edellyttää kolmea vaihetta:

- Luo  **yhteensopivuus käytäntöä**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), jotta voit määrittää asetukset, joiden on täytyttävä, ennen kuin laite katsotaan yhteensopivaksi. Esimerkiksi laitteessa on oltava vähintään 6-numeroinen PIN-koodi, ennen kuin sen katsotaan olevan yhteensopiva.
- Luo **Ehdollinen käyttö oikeus menettely**  , joka määrittää, mitä resursseja suojellaan, ja mitkä ehdot on täytettävä, jotta nämä resurssit ovat käytettävissä.  [Esimerkiksi](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  laitteen on oltava yhteensopiva ennen yritys sähkö postin käyttöä.
- Varmista, että sekä **yhteensopivuus käytännöt**  että  **ehdolliset käyttö oikeus käytännöt**  on kohdistettu halutulle käyttäjä ryhmälle. Tämä saattaa edellyttää tiettyjen käyttäjä ryhmien luomista Azure Active Directoryyn.

**Hyödyllisiä linkkejä:**

[Laitteen yhteensopivuuden yleiskatsaus](https://docs.microsoft.com/intune/device-compliance-get-started)

[Varmenteiden myöntäjän vian määritys](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Vian määritys käytännöt](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Jos haluat suojata sähkö postin (Exchange Online) yhteensopimattomien laitteiden käytöltä, molempia asia kirjoja on noudatettava:

1. [Sähkö postin käyttö oikeuksien suojaaminen EAS-laitteiden avulla](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Sähkö postin käyttö oikeuksien suojaaminen nykyaikaisilla todennus ohjelmilla, kuten Outlookilla](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)