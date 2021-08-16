---
title: Ehdollinen käyttöoikeus Intunen avulla
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c24451fba8b8ab8fe7a1778bb292dec6678e1ef487076d27458c9aeb4963c683
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069709"
---
# <a name="conditional-access-with-intune"></a>Ehdollinen käyttöoikeus Intunen avulla

Ehdollisen  **käyttöoikeuden käyttäminen**  Intunen kanssa edellyttää kolmea vaihetta:

- Luo **yhteensopivuuskäytäntö** ([Android,](https://docs.microsoft.com/intune/compliance-policy-create-android) [iOS,](https://docs.microsoft.com/intune/compliance-policy-create-ios) [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) ja määritä asetukset, jotka on täytettävä, ennen kuin laite on yhteensopiva. Laitteessa on esimerkiksi oltava vähintään kuusinumeroinen PIN-koodi, ennen kuin se on yhteensopiva.
- Luo **ehdollisen käyttöoikeuden käytäntö,**  joka määrittää suojattavat resurssit ja sen, mitkä ehdot on täytettävä, jotta resursseja voi käyttää.  [Laitteen on esimerkiksi](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  oltava yhteensopiva, ennen kuin se voi käyttää yrityksen sähköpostia.
- Varmista, **että sekä yhteensopivuuskäytännöt**  **että ehdolliset käyttöoikeuskäytännöt**  kohdennetaan halutuille käyttäjäryhmille. Tämä voi edellyttää tiettyjen käyttäjäryhmien luomista Azure Active Directory.

**Hyödyllisiä linkkejä:**

[Laitteen yhteensopivuuden yleiskatsaus](https://docs.microsoft.com/intune/device-compliance-get-started)

[Varmenteiden myöntäjän vianmääritys](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Vianmäärityskäytäntö](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Jotta sähköpostin (Exchange online-tilassa) ei-laitekäyttö olisi käytettävissä, molemmat asiakirjat on seurattava seuraavasti:

1. [Sähköpostin käytön suojaaminen laitteilla EAS:n avulla](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Sähköpostin käytön suojaaminen laitteilla modernin varmennusasiakkaan, kuten Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)