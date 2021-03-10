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
# <a name="using-conditional-access-with-intune"></a><span data-ttu-id="13be8-102">Ehdollisen käyttöoikeuden käyttäminen Intunen kanssa</span><span class="sxs-lookup"><span data-stu-id="13be8-102">Using Conditional Access with Intune</span></span>

<span data-ttu-id="13be8-103">Ehdollisen käyttöoikeuden käyttäminen Intunen kanssa edellyttää kolmea vaihetta:</span><span class="sxs-lookup"><span data-stu-id="13be8-103">Using Conditional Access with Intune requires 3 steps:</span></span>

- [<span data-ttu-id="13be8-104">Luo yhteensopivuuskäytäntö, joka määrittää asetukset, jotka on täytettävä, ennen kuin laite on yhteensopiva. Laitteessa on esimerkiksi oltava vähintään kuusinumeroinen nasta, ennen kuin se on yhteensopiva.</span><span class="sxs-lookup"><span data-stu-id="13be8-104">Create a Compliance Policy to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [<span data-ttu-id="13be8-105">Luo ehdollinen käyttöoikeuskäytäntö, joka määrittää, mitä resursseja suojataan ja mitkä ehdot on täytettävä, jotta resursseja voi käyttää. Laitteen on esimerkiksi oltava yhteensopiva, ennen kuin se voi käyttää yrityksen sähköpostia.</span><span class="sxs-lookup"><span data-stu-id="13be8-105">Create a Conditional Access Policy that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span>](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [<span data-ttu-id="13be8-106">Varmista, että sekä yhteensopivuuskäytännöt että ehdolliset käyttöoikeuskäytännöt on kohdennettu halutuille käyttäjäryhmille. Tämä voi edellyttää tiettyjen käyttäjäryhmien luomista Azure Active Directoryssa.</span><span class="sxs-lookup"><span data-stu-id="13be8-106">Ensure both Compliance Policies and Conditional Access Policies are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[<span data-ttu-id="13be8-107">Lisätietoja...</span><span class="sxs-lookup"><span data-stu-id="13be8-107">Read more...</span></span>](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
