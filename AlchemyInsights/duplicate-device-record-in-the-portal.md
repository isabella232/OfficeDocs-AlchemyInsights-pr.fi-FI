---
title: Laitetietueen kaksoiskappale portaalissa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2020
ms.locfileid: "43789859"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="748d8-102">Laitetietueen kaksoiskappale portaalissa</span><span class="sxs-lookup"><span data-stu-id="748d8-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="748d8-103">Laitteelle voi olla portaalissa näkyvissä 2 tietuetta, jos laite ei ilmoita oikein yhteishallintatilaa Configuration Manager -sivustolle.</span><span class="sxs-lookup"><span data-stu-id="748d8-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="748d8-104">Jos haluat tarkistaa laitteen yhteishallintatilan, katso laitteen **Yhteishallinta**-sarake Configuration Manager -konsolista.</span><span class="sxs-lookup"><span data-stu-id="748d8-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="748d8-105">Jos sarake ei ole näkyvissä, voit lisätä sen napsauttamalla jotakin sarakkeen otsikoista hiiren kakkospainikkeella ja valitsemalla sen luettelosta.</span><span class="sxs-lookup"><span data-stu-id="748d8-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="748d8-106">Yhteishallinta-arvon pitää olla **Kyllä**.</span><span class="sxs-lookup"><span data-stu-id="748d8-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="748d8-107">Jos arvo on **Ei**, avaa Configuration Manager -asiakassovellus asiakaslaitteesta ja tarkista **Yhteishallinta**-ominaisuus Yleiset-välilehdeltä.</span><span class="sxs-lookup"><span data-stu-id="748d8-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="748d8-108">Jos arvo on **Käytössä**, tämä tarkoittaa ongelmia asiakasviestinnässä hallintapisteissä.</span><span class="sxs-lookup"><span data-stu-id="748d8-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="748d8-109">Tarkista laitteen**CcmMessaging. log** mahdollisten yhteysongelmien tutkimiseksi.</span><span class="sxs-lookup"><span data-stu-id="748d8-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="748d8-110">Jos arvo on **Pois käytöstä** ja laite on rekisteröity Intunessa, varmista, että laite on saanut yhteishallintakäytännön tarkistamalla laitteesta lokin**CoManagementHandler.log**.</span><span class="sxs-lookup"><span data-stu-id="748d8-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
