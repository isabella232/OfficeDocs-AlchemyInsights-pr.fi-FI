---
title: Ehdollisen käyttöoikeuden käyttäminen Intunen kanssa
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
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693574"
---
# <a name="using-conditional-access-with-intune"></a>Ehdollisen käyttöoikeuden käyttäminen Intunen kanssa

Ehdollisen käyttöoikeuden käyttäminen Intunen kanssa edellyttää kolmea vaihetta:

- [Luo yhteensopivuuskäytäntö, joka määrittää asetukset, jotka on täytettävä, ennen kuin laite on yhteensopiva. Laitteessa on esimerkiksi oltava vähintään kuusinumeroinen nasta, ennen kuin se on yhteensopiva.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Luo ehdollinen käyttöoikeuskäytäntö, joka määrittää, mitä resursseja suojataan ja mitkä ehdot on täytettävä, jotta resursseja voi käyttää. Laitteen on esimerkiksi oltava yhteensopiva, ennen kuin se voi käyttää yrityksen sähköpostia.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Varmista, että sekä yhteensopivuuskäytännöt että ehdolliset käyttöoikeuskäytännöt on kohdennettu halutuille käyttäjäryhmille. Tämä voi edellyttää tiettyjen käyttäjäryhmien luomista Azure Active Directoryssa.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Lisätietoja...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
