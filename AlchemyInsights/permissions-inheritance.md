---
title: Käyttöoikeuksien periytyminen
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bb5c440a-ca70-4dc6-b517-688e80551101
ms.openlocfilehash: 791085593433dcad9b800fdea8c7ea4a878604e7
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581048"
---
# <a name="how-permissions-inheritance-works-in-sharepoint"></a><span data-ttu-id="950eb-102">Käyttöoikeuksien periytymisen toiminta SharePointissa</span><span class="sxs-lookup"><span data-stu-id="950eb-102">How permissions inheritance works in SharePoint</span></span>

<span data-ttu-id="950eb-103">Oletusarvon mukaan SharePointin käyttöoikeudet periytyvät ylemmästä hierarkiasta.</span><span class="sxs-lookup"><span data-stu-id="950eb-103">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="950eb-104">Tiedosto perii siis käyttöoikeudet kansiosta, joka perii sen käyttöoikeudet kirjastosta, mikä perii sen käyttöoikeudet sivustosta, mikä perii sen käyttöoikeudet sivustokokoelmasta.</span><span class="sxs-lookup"><span data-stu-id="950eb-104">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site, which inherits its permissions from the site collection.</span></span>
  
<span data-ttu-id="950eb-105">Lisätietoja yksilöllisten käyttöoikeuksien poistamisesta ja periytymisen [palauttamisesta on ohjeaiheessa Luettelon tai kirjaston käyttöoikeuksien muokkaaminen ja hallinta](https://go.microsoft.com/fwlink/?linkid=869946).</span><span class="sxs-lookup"><span data-stu-id="950eb-105">For info about removing unique permissions and restoring inheritance, see [Edit and manage permissions for a list or library](https://go.microsoft.com/fwlink/?linkid=869946).</span></span>
  

