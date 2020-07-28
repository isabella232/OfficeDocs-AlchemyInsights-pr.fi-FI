---
title: Tietojen poistaminen ja laitteiden pyyhkiminen Intunesta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439650"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="3b20c-102">Tietojen poistaminen ja laitteiden pyyhkiminen Intunesta</span><span class="sxs-lookup"><span data-stu-id="3b20c-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="3b20c-103">Device Retire- ja Device Wipe -etätoimintoja voidaan käyttää Intune-järjestelmän hallinnoimien yritystietojen poistamiseen tai tehdasasetusten palauttamiseen ja laitteen oletusasetusten palauttamiseen.</span><span class="sxs-lookup"><span data-stu-id="3b20c-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="3b20c-104">Kirjaudu Microsoft 365 Device Managementiin ja valitse **Laitteet**  >  **kaikki laitteet**.</span><span class="sxs-lookup"><span data-stu-id="3b20c-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="3b20c-105">Valitse laite, jonka haluat pyyhkiä.</span><span class="sxs-lookup"><span data-stu-id="3b20c-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="3b20c-106">Valitse etätyhjennuksen tyyppi, jonka haluat tehdä.</span><span class="sxs-lookup"><span data-stu-id="3b20c-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="3b20c-107">Poista käytöstä vain organisaatiotiedot, kun taas täydet pyyhkeet palauttavat laitteen tehdasasetuksiinsa.</span><span class="sxs-lookup"><span data-stu-id="3b20c-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="3b20c-108">Vahvista valitsemalla **Kyllä.**</span><span class="sxs-lookup"><span data-stu-id="3b20c-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="3b20c-109">Laitetoiminnon tila näkyy Odottavassa tilassa, kunnes pyyhi on valmis.</span><span class="sxs-lookup"><span data-stu-id="3b20c-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="3b20c-110">Kun toiminto on valmis, et enää näe mobiililaitetta hallitun laitteen luettelossa.</span><span class="sxs-lookup"><span data-stu-id="3b20c-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="3b20c-111">**Huomautus** Yrityksen tietoja ei voi poistaa Azure AD:hen liitetyistä laitteista.</span><span class="sxs-lookup"><span data-stu-id="3b20c-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="3b20c-112">Täydelliset tiedot Käytöstä- ja Pyyhi-toimintojen vaikutuksesta, mukaan lukien säilytetyt ja poistetut toiminnot, on [ohjeaiheessa Laitteiden poistaminen pyyhkimällä, poistamalla käytöstä tai poistamalla laitteen manuaalisesti](https://docs.microsoft.com/intune/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="3b20c-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="3b20c-113">Lisätietoja kaikkien tietojen poistamisesta macOS-laitteesta on [ohjeaiheessa Kaikkien tietojen poistaminen macOS-laitteesta](https://docs.microsoft.com/intune/device-erase).</span><span class="sxs-lookup"><span data-stu-id="3b20c-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>