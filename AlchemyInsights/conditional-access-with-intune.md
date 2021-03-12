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
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704783"
---
# <a name="conditional-access-with-intune"></a>Ehdollinen käyttöoikeus Intunen avulla

Ehdollisen  **käyttöoikeuden käyttäminen**  Intunen kanssa edellyttää kolmea vaihetta:

- Luo  **yhteensopivuuskäytäntö** [(Android,](https://docs.microsoft.com/intune/compliance-policy-create-android)  [iOS,](https://docs.microsoft.com/intune/compliance-policy-create-ios)  [Windows)](https://docs.microsoft.com//intune/compliance-policy-create-windows)ja määritä asetukset, jotka on täytettävä, ennen kuin laite on yhteensopiva. Laitteessa on esimerkiksi oltava vähintään kuusinumeroinen nasta, ennen kuin se on yhteensopiva.
- Luo **ehdollinen käyttöoikeuskäytäntö,**  joka määrittää, mitä resursseja suojataan ja mitkä ehdot on täytettävä, jotta resursseja voi käyttää.  [Laitteen on](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  esimerkiksi oltava yhteensopiva, ennen kuin se voi käyttää yrityksen sähköpostia.
- Varmista, **että sekä yhteensopivuuskäytännöt**  **että ehdolliset**  käyttöoikeuskäytännöt on kohdennettu halutuille käyttäjäryhmille. Tämä voi edellyttää tiettyjen käyttäjäryhmien luomista Azure Active Directoryssa.

**Hyödyllisiä linkkejä:**

[Laitteen yhteensopivuuden yleiskatsaus](https://docs.microsoft.com/intune/device-compliance-get-started)

[Varmenteiden myöntäjän vianmääritys](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Vianmäärityskäytäntö](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Jotta sähköposti (Exchange Online) voidaan suojata muilta kuin epätavalaisilta laitteilta, molempien asiakirjojen on oltava seuraavat:

1. [Sähköpostin käytön suojaaminen EAS-laitteella](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Sähköpostin käytön suojaaminen laitteista, kuten Outlookista, modernin varmennusohjelman avulla](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)