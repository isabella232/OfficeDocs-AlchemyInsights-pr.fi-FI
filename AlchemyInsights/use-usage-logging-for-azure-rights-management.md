---
title: Käyttölokin käyttäminen Azure-oikeuksien hallinnassa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5506"
- "9002281"
ms.openlocfilehash: 606fcdc5394edab26c60925af28cf2d938aac172
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/03/2020
ms.locfileid: "46555125"
---
# <a name="use-usage-logging-for-azure-rights-management"></a><span data-ttu-id="0661b-102">Käyttölokin käyttäminen Azure-oikeuksien hallinnassa</span><span class="sxs-lookup"><span data-stu-id="0661b-102">Use usage logging for Azure Rights Management</span></span>

<span data-ttu-id="0661b-103">Oletusarvon mukaan suojauksen käyttöloki on käytössä kaikille asiakkaille.</span><span class="sxs-lookup"><span data-stu-id="0661b-103">By default, protection usage logging is enabled for all customers.</span></span> <span data-ttu-id="0661b-104">Lokit kirjoitetaan vuokraajan Azure-tallennustilassa.</span><span class="sxs-lookup"><span data-stu-id="0661b-104">Logs are written as a series of blobs in Azure storage for your tenant.</span></span> <span data-ttu-id="0661b-105">Suojaustoiminnon jälkeen useimpien lokien näkyminen saattaa kestää jopa 15 minuuttia.</span><span class="sxs-lookup"><span data-stu-id="0661b-105">After a protection action, it might take up to 15 minutes for most logs to appear.</span></span>

<span data-ttu-id="0661b-106">Suojauskäyttölokien avulla voit</span><span class="sxs-lookup"><span data-stu-id="0661b-106">You can use protection usage logs to:</span></span>

- <span data-ttu-id="0661b-107">Analysoi liiketoiminnan kävijätietoja</span><span class="sxs-lookup"><span data-stu-id="0661b-107">Analyze business insights</span></span>

- <span data-ttu-id="0661b-108">Valvo väärinkäyttöä</span><span class="sxs-lookup"><span data-stu-id="0661b-108">Monitor for abuse</span></span>

- <span data-ttu-id="0661b-109">Rikosteknisen analyysin suorittaminen</span><span class="sxs-lookup"><span data-stu-id="0661b-109">Perform forensic analysis</span></span>

<span data-ttu-id="0661b-110">Lisätietoja on kohdassa [Azure Information Protectionin suojauksen käytön kirjaaminen ja analysointi](https://docs.microsoft.com/azure/information-protection/log-analyze-usage).</span><span class="sxs-lookup"><span data-stu-id="0661b-110">For more information, see [Logging and analyzing the protection usage from Azure Information Protection](https://docs.microsoft.com/azure/information-protection/log-analyze-usage).</span></span>

<span data-ttu-id="0661b-111">Lisätietoja asiakkaiden käyttökirjauksesta on kohdassa [Järjestelmänvalvojan opas: Azure Information Protection -asiakastiedostot ja asiakkaan käyttöloki](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-files-and-logging).</span><span class="sxs-lookup"><span data-stu-id="0661b-111">For information about client usage logging, see [Admin Guide: Azure Information Protection client files and client usage logging](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-files-and-logging).</span></span>

<span data-ttu-id="0661b-112">Lisätietoja on seuraavissa ohjeissa:</span><span class="sxs-lookup"><span data-stu-id="0661b-112">For additional information, see:</span></span>

- <span data-ttu-id="0661b-113">[Azure-tietojen suojausvaatimukset](https://docs.microsoft.com/azure/information-protection/get-started/requirements).</span><span class="sxs-lookup"><span data-stu-id="0661b-113">[Azure Information Protection requirements](https://docs.microsoft.com/azure/information-protection/get-started/requirements).</span></span>
    
- <span data-ttu-id="0661b-114">[Opetusohjelma: Azure Information Protection -käytäntöasetusten määrittäminen ja uuden tunnisteen luominen](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial).</span><span class="sxs-lookup"><span data-stu-id="0661b-114">[Tutorial: Configure Azure Information Protection policy settings and create a new label](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial).</span></span>