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
ms.openlocfilehash: 23afea21668191093d612d68ca6e9ab2a844f4a14977631d33f4fd956fc3c4e7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005771"
---
# <a name="using-conditional-access-with-intune"></a>Ehdollisen käyttöoikeuden käyttäminen Intunen kanssa

Ehdollisen käyttöoikeuden käyttäminen Intunen kanssa edellyttää kolmea vaihetta:

- [Luo yhteensopivuuskäytäntö, joka määrittää asetukset, jotka on täytettävä, ennen kuin laite on yhteensopiva. Laitteessa on esimerkiksi oltava vähintään kuusinumeroinen PIN-koodi, ennen kuin se on yhteensopiva.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Luo ehdollisen käyttöoikeuden käytäntö, joka määrittää suojattavat resurssit ja sen, mitkä ehdot on täytettävä, jotta resursseja voi käyttää. Laitteen on esimerkiksi oltava yhteensopiva, ennen kuin se voi käyttää yrityksen sähköpostia.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Varmista, että sekä yhteensopivuuskäytännöt että ehdolliset käyttöoikeuskäytännöt kohdennetaan halutuille käyttäjäryhmille. Tämä voi edellyttää tiettyjen käyttäjäryhmien luomista Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Lisätietoja...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
