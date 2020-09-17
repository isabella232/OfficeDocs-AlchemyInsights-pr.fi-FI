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
# <a name="conditional-access-with-intune"></a><span data-ttu-id="25f78-102">Ehdollinen käyttäminen Intunella</span><span class="sxs-lookup"><span data-stu-id="25f78-102">Conditional Access with Intune</span></span>

<span data-ttu-id="25f78-103">**Ehdollisen käyttö oikeuden** käyttäminen Intunella edellyttää kolmea vaihetta:</span><span class="sxs-lookup"><span data-stu-id="25f78-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="25f78-104">Luo  **yhteensopivuus käytäntöä**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), jotta voit määrittää asetukset, joiden on täytyttävä, ennen kuin laite katsotaan yhteensopivaksi.</span><span class="sxs-lookup"><span data-stu-id="25f78-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="25f78-105">Esimerkiksi laitteessa on oltava vähintään 6-numeroinen PIN-koodi, ennen kuin sen katsotaan olevan yhteensopiva.</span><span class="sxs-lookup"><span data-stu-id="25f78-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="25f78-106">Luo **Ehdollinen käyttö oikeus menettely**  , joka määrittää, mitä resursseja suojellaan, ja mitkä ehdot on täytettävä, jotta nämä resurssit ovat käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="25f78-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="25f78-107">[Esimerkiksi](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  laitteen on oltava yhteensopiva ennen yritys sähkö postin käyttöä.</span><span class="sxs-lookup"><span data-stu-id="25f78-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="25f78-108">Varmista, että sekä **yhteensopivuus käytännöt**  että  **ehdolliset käyttö oikeus käytännöt**  on kohdistettu halutulle käyttäjä ryhmälle.</span><span class="sxs-lookup"><span data-stu-id="25f78-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="25f78-109">Tämä saattaa edellyttää tiettyjen käyttäjä ryhmien luomista Azure Active Directoryyn.</span><span class="sxs-lookup"><span data-stu-id="25f78-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="25f78-110">**Hyödyllisiä linkkejä:**</span><span class="sxs-lookup"><span data-stu-id="25f78-110">**Helpful links:**</span></span>

[<span data-ttu-id="25f78-111">Laitteen yhteensopivuuden yleiskatsaus</span><span class="sxs-lookup"><span data-stu-id="25f78-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="25f78-112">Varmenteiden myöntäjän vian määritys</span><span class="sxs-lookup"><span data-stu-id="25f78-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="25f78-113">Vian määritys käytännöt</span><span class="sxs-lookup"><span data-stu-id="25f78-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="25f78-114">Jos haluat suojata sähkö postin (Exchange Online) yhteensopimattomien laitteiden käytöltä, molempia asia kirjoja on noudatettava:</span><span class="sxs-lookup"><span data-stu-id="25f78-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="25f78-115">Sähkö postin käyttö oikeuksien suojaaminen EAS-laitteiden avulla</span><span class="sxs-lookup"><span data-stu-id="25f78-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="25f78-116">Sähkö postin käyttö oikeuksien suojaaminen nykyaikaisilla todennus ohjelmilla, kuten Outlookilla</span><span class="sxs-lookup"><span data-stu-id="25f78-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)