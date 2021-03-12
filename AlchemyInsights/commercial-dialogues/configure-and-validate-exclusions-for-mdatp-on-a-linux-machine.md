---
title: MDATP-poikkeuksien määrittäminen ja vahvistaminen Linux-koneessa
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
- "9000760"
- "7391"
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746025"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="75495-102">MDATP-poikkeuksien määrittäminen ja vahvistaminen Linux-koneessa</span><span class="sxs-lookup"><span data-stu-id="75495-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="75495-103">Voit jättää tietyt tiedostot, kansiot, prosessit ja prosessi avatut tiedostot pois MDATP-skannauksista.</span><span class="sxs-lookup"><span data-stu-id="75495-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="75495-104">Poikkeukset auttavat estämään ohjelmistojen ja tiedostojen virheellisen tunnistuksen, joka on yksilöllinen tai mukautettu organisaatiollesi.</span><span class="sxs-lookup"><span data-stu-id="75495-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="75495-105">Poikkeukset auttavat myös MDATP:n aiheuttamien suorituskykyongelmien lieventämiseen.</span><span class="sxs-lookup"><span data-stu-id="75495-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="75495-106">Lisätietoja on kohdassa [MDATP for Linuxin poikkeusten](https://go.microsoft.com/fwlink/?linkid=2144517)määrittäminen ja vahvistaminen.</span><span class="sxs-lookup"><span data-stu-id="75495-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="75495-107">Tässä artikkelissa kuvatut poikkeukset eivät koske muita MDATP for Linuxin ominaisuuksia, kuten päätepisteiden tunnistusta ja vastausta.</span><span class="sxs-lookup"><span data-stu-id="75495-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="75495-108">Tässä artikkelissa kuvattujen menetelmien avulla ohitettavat tiedostot voivat silti käynnistää EDR-ilmoituksia ja muita tunnistusominaisuuksia.</span><span class="sxs-lookup"><span data-stu-id="75495-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>
