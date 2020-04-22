---
title: Käytön rajoittaminen SharePointissa tai OneDrivessa
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: ed8e97b20c96a7b46995c969074cc4cef3a787d9
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715881"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="62f31-102">Käytön rajoittaminen SharePointissa tai OneDrivessa</span><span class="sxs-lookup"><span data-stu-id="62f31-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="62f31-103">SharePointissa ja OneDrivessa voit rajoittaa kohteiden, kuten tiedostojen, kansioiden ja luetteloiden, käyttöä myöntämällä käyttöoikeuden vain ryhmille tai henkilöille, joilla haluat käyttää.</span><span class="sxs-lookup"><span data-stu-id="62f31-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="62f31-104">Oletusarvon mukaan SharePointin käyttöoikeudet periytyvät hierarkiassa ylemmältä.</span><span class="sxs-lookup"><span data-stu-id="62f31-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="62f31-105">Näin ollen tiedosto perii käyttöoikeudet kansiosta, joka perii sen käyttöoikeudet kirjastosta, joka perii sen käyttöoikeudet sivustosta.</span><span class="sxs-lookup"><span data-stu-id="62f31-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="62f31-106">Voit jakaa korkeammalla tasolla (esimerkiksi jakamalla koko sivuston) ja sitten jakaa periytymisen, jos et halua jakaa kaikkia sivuston kohteita.</span><span class="sxs-lookup"><span data-stu-id="62f31-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="62f31-107">Emme kuitenkaan suosittele tätä, koska se tekee käyttöoikeuksien säilyttämisestä monimutkaisempaa ja hämmentävämpää tulevaisuudessa.</span><span class="sxs-lookup"><span data-stu-id="62f31-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="62f31-108">Tässä mitä voisit tehdä sen sijaan:</span><span class="sxs-lookup"><span data-stu-id="62f31-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="62f31-109">Jos esimerkiksi haluat jakaa kansion koko sisällön yhtä tiedostoa lukuun ottamatta, siirrä tiedosto uuteen sijaintiin, jota ei ole jaettu.</span><span class="sxs-lookup"><span data-stu-id="62f31-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="62f31-110">Jos kansiossa on kaksi alikansiota ja haluat jakaa yhden alikansion ryhmien A ja B kanssa ja sallia vain toisen alikansion A-käyttöoikeuden, jaa pääkansio ryhmän A kanssa ja lisää ryhmä B ensimmäiseen alikansioon.</span><span class="sxs-lookup"><span data-stu-id="62f31-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="62f31-111">Tiedoston tai kansion jakamisen lopettaminen</span><span class="sxs-lookup"><span data-stu-id="62f31-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

