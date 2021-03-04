---
title: Tietojen ja laitteiden poistaminen Intunesta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416310"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="c7435-102">Tietojen ja laitteiden poistaminen Intunesta</span><span class="sxs-lookup"><span data-stu-id="c7435-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="c7435-103">Laitteen käytöstä poistaminen ja laitteen tietojen poistaminen ovat etätoimintoja, joilla voidaan poistaa Intunen hallitsemia yritystietoja tai suorittaa tehdasasetusten palautus ja palauttaa laitteen oletusasetukset.</span><span class="sxs-lookup"><span data-stu-id="c7435-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="c7435-104">Kirjaudu sisään Microsoft 365 -laitteiden hallintaan ja siirry kohtaan **Laitteet** > **Kaikki laitteet**.</span><span class="sxs-lookup"><span data-stu-id="c7435-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="c7435-105">Valitse laite, jonka tiedot haluat poistaa.</span><span class="sxs-lookup"><span data-stu-id="c7435-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="c7435-106">Valitse, minkä tyyppistä etäpoistoa haluat käyttää.</span><span class="sxs-lookup"><span data-stu-id="c7435-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="c7435-107">Laitteen käytöstä poistaminen poistaa vain yrityksen tiedot, kun taas kaikkien tietojen poistaminen palauttaa laitteen tehdasasetukset.</span><span class="sxs-lookup"><span data-stu-id="c7435-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="c7435-108">Vahvista valitsemalla **Kyllä**.</span><span class="sxs-lookup"><span data-stu-id="c7435-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="c7435-109">Kunnes tietojen poistaminen on valmis, laitteen toiminnon tila näyttää, että *Käytöstä poisto odottaa*.</span><span class="sxs-lookup"><span data-stu-id="c7435-109">Until the wipe finishes, the Device action status shows as *Retire Pending*.</span></span>
    <span data-ttu-id="c7435-110">Kun toiminto on valmis, mobiililaite ei näy enää hallittujen laitteiden listassa.</span><span class="sxs-lookup"><span data-stu-id="c7435-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

> [!NOTE]
> <span data-ttu-id="c7435-111">Yritystietoja ei voi poistaa laitteista, jotka on LIITETTY Azure AD:hen.</span><span class="sxs-lookup"><span data-stu-id="c7435-111">Company data can't be removed from devices JOINED to Azure AD.</span></span> 

<span data-ttu-id="c7435-112">Lisätietoja laitteen käytöstä poistamisen ja laitteen tietojen poistamisen vaikutuksista, mukaan lukien siitä, mitä säilytetään ja mitä poistetaan, löytyy seuraavista ohjeista:</span><span class="sxs-lookup"><span data-stu-id="c7435-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see following documentation:</span></span>

- <span data-ttu-id="c7435-113">[Poista laite poistamalla se käytöstä, poistamalla laitteen tiedot tai poistamalla laitteen rekisteröinti manuaalisesti](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="c7435-113">[Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span></span>
- [<span data-ttu-id="c7435-114">Kuinka poistaa vain yritystiedot Intunen hallitsemista sovelluksista</span><span class="sxs-lookup"><span data-stu-id="c7435-114">How to wipe only corporate data from Intune-managed apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- <span data-ttu-id="c7435-115">[Poista kaikki tiedot macOS-laitteesta](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span><span class="sxs-lookup"><span data-stu-id="c7435-115">[Erase all data from a macOS device](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span></span>