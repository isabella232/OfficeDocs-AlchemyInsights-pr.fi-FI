---
title: Co-Management
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1556"
- "9000080"
ms.openlocfilehash: fe7dcebf847fbd7d91632e93e2253bf62ac659aa
ms.sourcegitcommit: 4ed431b2e1aed26d07bd7eba282531537d29ad0e
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/30/2019
ms.locfileid: "40910266"
---
# <a name="co-management"></a><span data-ttu-id="45a85-102">Co-Management</span><span class="sxs-lookup"><span data-stu-id="45a85-102">Co-management</span></span>

<span data-ttu-id="45a85-103">**Edellytykset config Manager Hybrid-palvelusta Intune-siirtymille**</span><span class="sxs-lookup"><span data-stu-id="45a85-103">**Prerequisites for migrating from Config Manager Hybrid to Intune**</span></span>

- <span data-ttu-id="45a85-104">Tarkista [Tämä artikkeli](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-hybridmdm-to-intunesa).</span><span class="sxs-lookup"><span data-stu-id="45a85-104">Review [this article](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-hybridmdm-to-intunesa).</span></span>
- <span data-ttu-id="45a85-105">[Lisää Intune-lisenssi käyttäjilleen](https://docs.microsoft.com/intune/licenses-assign).</span><span class="sxs-lookup"><span data-stu-id="45a85-105">[Add an Intune license to your users](https://docs.microsoft.com/intune/licenses-assign).</span></span>
- <span data-ttu-id="45a85-106">Käytä [Edge-selainta](https://www.microsoft.com/windows/microsoft-edge) , kun määrität yhteishallintaa.</span><span class="sxs-lookup"><span data-stu-id="45a85-106">Use the [Edge browser](https://www.microsoft.com/windows/microsoft-edge) when configuring Co-management.</span></span>

<span data-ttu-id="45a85-107">**Miten asennan config Manager-asiakkaan Intune-hallittuja laitteita varten**</span><span class="sxs-lookup"><span data-stu-id="45a85-107">**How to I install the Config Manager client on Intune-managed devices**</span></span>

<span data-ttu-id="45a85-108">Katso [Intune MDM-hallitut Windows-laitteet](https://docs.microsoft.com/sccm/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm).</span><span class="sxs-lookup"><span data-stu-id="45a85-108">See [Intune MDM-managed Windows devices](https://docs.microsoft.com/sccm/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm).</span></span>

<span data-ttu-id="45a85-109">**Entä jos haluan vain muuttaa MDM-viran omaista?**</span><span class="sxs-lookup"><span data-stu-id="45a85-109">**What if I just want to change MDM authority?**</span></span>

<span data-ttu-id="45a85-110">MDM-viran omaista voidaan muuttaa avaamatta tuki tapausta.</span><span class="sxs-lookup"><span data-stu-id="45a85-110">MDM Authority can be changed without opening a support case.</span></span> <span data-ttu-id="45a85-111">Lue seuraavat ohjeet, jotka auttavat MDM-viran omaisen muuttamisessa:</span><span class="sxs-lookup"><span data-stu-id="45a85-111">Please review the following documentation to assist in changing your MDM authority:</span></span>
- [<span data-ttu-id="45a85-112">Vaihda MDM-auktoriteetti config Managerista Intune-itsenäiseksi</span><span class="sxs-lookup"><span data-stu-id="45a85-112">Change MDM Authority from Config Manager to Intune standalone</span></span>](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-change-mdm-authority)
- [<span data-ttu-id="45a85-113">Vaihda MDM-auktoriteetti Intune erillispalvelusta config Manageriin</span><span class="sxs-lookup"><span data-stu-id="45a85-113">Change MDM Authority from Intune standalone to Config Manager</span></span>](https://docs.microsoft.com/intune-classic/deploy-use/prerequisites-for-enrollment#what-to-do-if-you-choose-the-wrong-mdm-authority-setting)