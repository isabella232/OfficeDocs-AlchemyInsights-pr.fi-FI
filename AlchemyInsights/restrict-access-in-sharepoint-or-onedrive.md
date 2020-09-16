---
title: Käytön rajoittaminen SharePointissa tai OneDrivessa
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720679"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="c0959-102">Käytön rajoittaminen SharePointissa tai OneDrivessa</span><span class="sxs-lookup"><span data-stu-id="c0959-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="c0959-103">SharePointin ja OneDriven avulla voit rajoittaa tiedostojen, kansioiden ja luetteloiden kaltaisia kohteita myöntämällä vain ryhmille tai henkilöille, joille haluat käyttää Accessia.</span><span class="sxs-lookup"><span data-stu-id="c0959-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="c0959-104">SharePointin käyttö oikeudet periytyvät oletusarvoisesti ylemmäksi hierarkiassa.</span><span class="sxs-lookup"><span data-stu-id="c0959-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="c0959-105">Tiedosto perii sen käyttö oikeudet kansiosta, jolloin sen käyttö oikeudet periytyvät kirjastosta, jolloin sen käyttö oikeudet periytyvät sivustosta.</span><span class="sxs-lookup"><span data-stu-id="c0959-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="c0959-106">Voit jakaa sen korkeamman tason (esimerkiksi jakamalla koko sivuston) ja katkaista periytymisen, jos et halua jakaa kaikkia sivuston kohteita.</span><span class="sxs-lookup"><span data-stu-id="c0959-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="c0959-107">Emme kuitenkaan suosittele tätä, koska se tekee käyttö oikeuksien säilyttämisestä monimutkaisemman ja sekavan tulevaisuudessa.</span><span class="sxs-lookup"><span data-stu-id="c0959-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="c0959-108">Voit tehdä sen sen sijaan seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="c0959-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="c0959-109">Jos haluat esimerkiksi jakaa koko kansion sisällön paitsi yhden tiedoston, siirrä tiedosto uuteen sijaintiin, jota ei jaeta.</span><span class="sxs-lookup"><span data-stu-id="c0959-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="c0959-110">Jos sinulla on kaksi alikansiota kansiossa ja haluat jakaa yhden alikansion ryhmien A ja B kanssa ja sallia vain ryhmän toisen alikansion käytön, Jaa pääkansio ryhmän A kanssa ja lisää ryhmä B ensimmäiseen alikansioon.</span><span class="sxs-lookup"><span data-stu-id="c0959-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="c0959-111">Tiedoston tai kansion jakamisen lopettaminen </span><span class="sxs-lookup"><span data-stu-id="c0959-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

