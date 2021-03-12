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
# <a name="conditional-access-with-intune"></a><span data-ttu-id="0e532-102">Ehdollinen käyttöoikeus Intunen avulla</span><span class="sxs-lookup"><span data-stu-id="0e532-102">Conditional Access with Intune</span></span>

<span data-ttu-id="0e532-103">Ehdollisen  **käyttöoikeuden käyttäminen**  Intunen kanssa edellyttää kolmea vaihetta:</span><span class="sxs-lookup"><span data-stu-id="0e532-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="0e532-104">Luo  **yhteensopivuuskäytäntö** [(Android,](https://docs.microsoft.com/intune/compliance-policy-create-android)  [iOS,](https://docs.microsoft.com/intune/compliance-policy-create-ios)  [Windows)](https://docs.microsoft.com//intune/compliance-policy-create-windows)ja määritä asetukset, jotka on täytettävä, ennen kuin laite on yhteensopiva.</span><span class="sxs-lookup"><span data-stu-id="0e532-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="0e532-105">Laitteessa on esimerkiksi oltava vähintään kuusinumeroinen nasta, ennen kuin se on yhteensopiva.</span><span class="sxs-lookup"><span data-stu-id="0e532-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="0e532-106">Luo **ehdollinen käyttöoikeuskäytäntö,**  joka määrittää, mitä resursseja suojataan ja mitkä ehdot on täytettävä, jotta resursseja voi käyttää.</span><span class="sxs-lookup"><span data-stu-id="0e532-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="0e532-107">[Laitteen on](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  esimerkiksi oltava yhteensopiva, ennen kuin se voi käyttää yrityksen sähköpostia.</span><span class="sxs-lookup"><span data-stu-id="0e532-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="0e532-108">Varmista, **että sekä yhteensopivuuskäytännöt**  **että ehdolliset**  käyttöoikeuskäytännöt on kohdennettu halutuille käyttäjäryhmille.</span><span class="sxs-lookup"><span data-stu-id="0e532-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="0e532-109">Tämä voi edellyttää tiettyjen käyttäjäryhmien luomista Azure Active Directoryssa.</span><span class="sxs-lookup"><span data-stu-id="0e532-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="0e532-110">**Hyödyllisiä linkkejä:**</span><span class="sxs-lookup"><span data-stu-id="0e532-110">**Helpful links:**</span></span>

[<span data-ttu-id="0e532-111">Laitteen yhteensopivuuden yleiskatsaus</span><span class="sxs-lookup"><span data-stu-id="0e532-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="0e532-112">Varmenteiden myöntäjän vianmääritys</span><span class="sxs-lookup"><span data-stu-id="0e532-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="0e532-113">Vianmäärityskäytäntö</span><span class="sxs-lookup"><span data-stu-id="0e532-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="0e532-114">Jotta sähköposti (Exchange Online) voidaan suojata muilta kuin epätavalaisilta laitteilta, molempien asiakirjojen on oltava seuraavat:</span><span class="sxs-lookup"><span data-stu-id="0e532-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="0e532-115">Sähköpostin käytön suojaaminen EAS-laitteella</span><span class="sxs-lookup"><span data-stu-id="0e532-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="0e532-116">Sähköpostin käytön suojaaminen laitteista, kuten Outlookista, modernin varmennusohjelman avulla</span><span class="sxs-lookup"><span data-stu-id="0e532-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)