---
title: Ehdollinen käyttö Intunen avulla
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931427"
---
# <a name="conditional-access-with-intune"></a>Ehdollinen käyttö Intunen avulla

**Ehdollisen käytön** käyttäminen Intunen kanssa edellyttää kolmea vaihetta:

- Luo **yhteensopivuuskäytäntö** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) määrittääksesi asetukset, jotka on täytettävä, ennen kuin laitetta pidetään vaatimusten mukaisena. Laitteessa on esimerkiksi oltava vähintään 6 numeron nasta, ennen kuin sitä pidetään vaatimusten mukaisena.
- Luo **ehdollinen käyttöoikeuskäytäntö,** joka määrittää, mitä resursseja suojataan ja mitkä ehdot on täytettävä, jotta näitä resursseja voidaan käyttää.  Laitteen on esimerkiksi oltava [yhteensopiva,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) ennen kuin se käyttää yrityksen sähköpostia.
- Varmista, että sekä **yhteensopivuuskäytännöt** että **ehdollisen käytön käytännöt** on kohdistettu halutuille käyttäjäryhmille. Tämä saattaa edellyttää tiettyjen käyttäjäryhmien luomista Azure Active Directoryyn.

**Hyödyllisiä linkkejä:**

[Laitteen yhteensopivuuden yleiskatsaus](https://docs.microsoft.com/intune/device-compliance-get-started)

[Myöntäjän myöntäjän vianmääritys](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Vianmäärityskäytäntö](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Jos haluat suojata sähköpostin (Exchange online) ei-yhteensopivien laitteiden käyttöolta, molempia asiakirjoja on noudatettava:

1. [Sähköpostin käytön suojaaminen laitteista EAS:n avulla](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Sähköpostin käytön suojaaminen laitteista nykyaikaisilla todennusasiakkailla, kuten Outlookilla](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)