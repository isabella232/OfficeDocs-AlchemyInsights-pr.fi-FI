---
title: Käyttö oikeuksien periytyminen
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 8/7/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bb5c440a-ca70-4dc6-b517-688e80551101
ms.openlocfilehash: 6322ca12902be2612f65b6388a650300b257a95e
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/25/2019
ms.locfileid: "36554942"
---
# <a name="how-permissions-inheritance-works-in-sharepoint"></a><span data-ttu-id="5b936-102">Miten käyttö oikeuksien periytyminen toimii SharePointissa</span><span class="sxs-lookup"><span data-stu-id="5b936-102">How permissions inheritance works in SharePoint</span></span>

<span data-ttu-id="5b936-103">Oletusarvoisesti SharePointin käyttö oikeudet periytyvät hierarkiassa ylemmiltä.</span><span class="sxs-lookup"><span data-stu-id="5b936-103">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="5b936-104">Joten tiedosto perit sen käyttö oikeudet kansiosta, joka perasti käyttö oikeudet kirjastosta, joka peri käyttö oikeudet sivustosta, joka peri käyttö oikeudet sivustokokoelmasta.</span><span class="sxs-lookup"><span data-stu-id="5b936-104">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site, which inherits its permissions from the site collection.</span></span>
  
<span data-ttu-id="5b936-105">Lisä tietoja yksilöllisten käyttö oikeuksien poistamisesta ja periytymisen palauttamisesta on kohdassa [luettelon tai kirjaston käyttö oikeuksien muokkaaminen ja hallinta](https://go.microsoft.com/fwlink/?linkid=869946).</span><span class="sxs-lookup"><span data-stu-id="5b936-105">For info about removing unique permissions and restoring inheritance, see [Edit and manage permissions for a list or library](https://go.microsoft.com/fwlink/?linkid=869946).</span></span>
  

