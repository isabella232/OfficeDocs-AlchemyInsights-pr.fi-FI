---
title: Microsoft Edgen asetaminen oletusselaimeksi toimialueeseen yhdistetyssä laitteessa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491587"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="741d6-102">Microsoft Edgen asetaminen oletusselaimeksi toimialueeseen yhdistetyssä laitteessa</span><span class="sxs-lookup"><span data-stu-id="741d6-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="741d6-103">Määritä Microsoft Edge oletusselaimeksi:</span><span class="sxs-lookup"><span data-stu-id="741d6-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="741d6-104">[Luo oletusarvoinen yhteyksien määritystiedosto](https://go.microsoft.com/fwlink/?linkid=2132437) ja tallenna se paikallisesti tai jaetuksi verkkoresurssiksi.</span><span class="sxs-lookup"><span data-stu-id="741d6-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="741d6-105">Avaa ryhmäkäytäntöeditori ja siirry sitten Tietokoneen **määrityksen**  >  **hallintamallit -ryhmässä**  >  **Windowsin osien**  >  **Resurssienhallintaan.**</span><span class="sxs-lookup"><span data-stu-id="741d6-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="741d6-106">Valitse **Määritä kytkennät -oletusmääritystiedosto.**</span><span class="sxs-lookup"><span data-stu-id="741d6-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="741d6-107">Valitse **Käytäntöasetus** ja valitse sitten **Käytössä.**</span><span class="sxs-lookup"><span data-stu-id="741d6-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="741d6-108">Kirjoita **Asetukset-kohdassa** kytkennän oletusmääritystiedoston sijainti ja valitse **sitten OK.**</span><span class="sxs-lookup"><span data-stu-id="741d6-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
