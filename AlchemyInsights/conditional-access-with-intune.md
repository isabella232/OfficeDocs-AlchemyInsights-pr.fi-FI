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
# <a name="conditional-access-with-intune"></a><span data-ttu-id="d078b-102">Ehdollinen käyttö Intunen avulla</span><span class="sxs-lookup"><span data-stu-id="d078b-102">Conditional Access with Intune</span></span>

<span data-ttu-id="d078b-103">**Ehdollisen käytön** käyttäminen Intunen kanssa edellyttää kolmea vaihetta:</span><span class="sxs-lookup"><span data-stu-id="d078b-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="d078b-104">Luo **yhteensopivuuskäytäntö** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) määrittääksesi asetukset, jotka on täytettävä, ennen kuin laitetta pidetään vaatimusten mukaisena.</span><span class="sxs-lookup"><span data-stu-id="d078b-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="d078b-105">Laitteessa on esimerkiksi oltava vähintään 6 numeron nasta, ennen kuin sitä pidetään vaatimusten mukaisena.</span><span class="sxs-lookup"><span data-stu-id="d078b-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="d078b-106">Luo **ehdollinen käyttöoikeuskäytäntö,** joka määrittää, mitä resursseja suojataan ja mitkä ehdot on täytettävä, jotta näitä resursseja voidaan käyttää.</span><span class="sxs-lookup"><span data-stu-id="d078b-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="d078b-107">Laitteen on esimerkiksi oltava [yhteensopiva,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) ennen kuin se käyttää yrityksen sähköpostia.</span><span class="sxs-lookup"><span data-stu-id="d078b-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="d078b-108">Varmista, että sekä **yhteensopivuuskäytännöt** että **ehdollisen käytön käytännöt** on kohdistettu halutuille käyttäjäryhmille.</span><span class="sxs-lookup"><span data-stu-id="d078b-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="d078b-109">Tämä saattaa edellyttää tiettyjen käyttäjäryhmien luomista Azure Active Directoryyn.</span><span class="sxs-lookup"><span data-stu-id="d078b-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="d078b-110">**Hyödyllisiä linkkejä:**</span><span class="sxs-lookup"><span data-stu-id="d078b-110">**Helpful links:**</span></span>

[<span data-ttu-id="d078b-111">Laitteen yhteensopivuuden yleiskatsaus</span><span class="sxs-lookup"><span data-stu-id="d078b-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="d078b-112">Myöntäjän myöntäjän vianmääritys</span><span class="sxs-lookup"><span data-stu-id="d078b-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="d078b-113">Vianmäärityskäytäntö</span><span class="sxs-lookup"><span data-stu-id="d078b-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="d078b-114">Jos haluat suojata sähköpostin (Exchange online) ei-yhteensopivien laitteiden käyttöolta, molempia asiakirjoja on noudatettava:</span><span class="sxs-lookup"><span data-stu-id="d078b-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="d078b-115">Sähköpostin käytön suojaaminen laitteista EAS:n avulla</span><span class="sxs-lookup"><span data-stu-id="d078b-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="d078b-116">Sähköpostin käytön suojaaminen laitteista nykyaikaisilla todennusasiakkailla, kuten Outlookilla</span><span class="sxs-lookup"><span data-stu-id="d078b-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)