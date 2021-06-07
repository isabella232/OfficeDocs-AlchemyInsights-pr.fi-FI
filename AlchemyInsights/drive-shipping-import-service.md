---
title: Levyaseman lähettäminen Microsoft 365 tuontipalvelussa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: 85d6e723e56b01fd9914165d8c9740f3b055947d
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731443"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a><span data-ttu-id="31c65-102">Levyaseman lähettäminen Microsoft 365 tuontipalvelussa</span><span class="sxs-lookup"><span data-stu-id="31c65-102">Drive shipping in the Microsoft 365 Import Service</span></span>

<span data-ttu-id="31c65-103">Käytä Drive-lähetystä kopioimalla PST:t kiintolevylle ja toimita sitten kiintolevy Microsoftille.</span><span class="sxs-lookup"><span data-stu-id="31c65-103">Use Drive shipping by copying PSTs to a hard drive and then shipping the hard drive to Microsoft.</span></span>

<span data-ttu-id="31c65-104">Työn käynnistäminen:</span><span class="sxs-lookup"><span data-stu-id="31c65-104">To start the job:</span></span>

1. <span data-ttu-id="31c65-105">Valitse Microsoft 365 hallinta **-kohdassa** **Tuo**.</span><span class="sxs-lookup"><span data-stu-id="31c65-105">In the Microsoft 365 Compliance Center under **Information Governance**, select **Import**.</span></span>

1. <span data-ttu-id="31c65-106">Valitse **Valitse tuontityön tyyppi** ja valitse sitten **Seuraava**.</span><span class="sxs-lookup"><span data-stu-id="31c65-106">Select **Choose import job type**, and then select **Next**.</span></span>

1. <span data-ttu-id="31c65-107">Jos haluat nähdä tämän tuontivaihtoehdon vaiheet, valitse **Lähetä kiintolevyt yhteen fyysiseen sijaintiimme**.</span><span class="sxs-lookup"><span data-stu-id="31c65-107">To see the steps for this import option, select **Ship hard drives to one of our physical locations**.</span></span>

<span data-ttu-id="31c65-108">Muista nämä asiat:</span><span class="sxs-lookup"><span data-stu-id="31c65-108">Here are some things to remember:</span></span>

- <span data-ttu-id="31c65-109">Sinulla on oltava postilaatikon tuonti- ja vientirooli määritettynä Exchange Online PST-tiedostojen Microsoft 365 postilaatikoihin.</span><span class="sxs-lookup"><span data-stu-id="31c65-109">You must be assigned the Mailbox Import Export role in Exchange Online to import PST files to Microsoft 365 mailboxes.</span></span>
<span data-ttu-id="31c65-110">Suorituskyky voi vaikuttaa yli 20 Gigatavun pst-laatuihin.</span><span class="sxs-lookup"><span data-stu-id="31c65-110">Performance might be impacted for PSTs larger than 20GB.</span></span>

- <span data-ttu-id="31c65-111">Vain 2,5 tuuman SSD-asemat ja 2,5 tuuman tai 3,5 tuuman sisäiset SATA II- ja SATA III -kiintolevyt ovat tuettuja.</span><span class="sxs-lookup"><span data-stu-id="31c65-111">Only 2.5-inch solid-state drives (SSDs) or 2.5-inch or 3.5-inch SATA II/III internal hard drives are supported.</span></span>
<span data-ttu-id="31c65-112">PST-tiedostoja sisältävä kiintolevy on salattava BitLocker.</span><span class="sxs-lookup"><span data-stu-id="31c65-112">Hard drive containing PST files must be encrypted with BitLocker.</span></span>

- <span data-ttu-id="31c65-113">PST-tiedostojen tuonti postilaatikoihin levyaseman Microsoft 365 on 2 Yhdysvaltain dollaria/ Gt tietoa.</span><span class="sxs-lookup"><span data-stu-id="31c65-113">The cost to import PST files to Microsoft 365 mailboxes using drive shipping is $2 USD per GB of data.</span></span>

<span data-ttu-id="31c65-114">Lisätietoja levyaseman lähettämisestä PST:n tuomiseen on kohdassa Organisaation PST-tiedostojen tuominen [levyaseman lähettämisen avulla.](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365)</span><span class="sxs-lookup"><span data-stu-id="31c65-114">For additional information on using the Drive shipping method for importing PSTs, see [Use drive shipping to import your organization's PST files](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).</span></span>