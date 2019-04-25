---
title: Kirjoita SharePoint- tai OneDrive käytön rajoittaminen
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e0fbec6eb269a173664e2b9a1efe6eefb527b96f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32383868"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="be13a-102">Kirjoita SharePoint- tai OneDrive käytön rajoittaminen</span><span class="sxs-lookup"><span data-stu-id="be13a-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="be13a-103">SharePoint-ja OneDrive voit rajoittaa kohteita, kuten tiedostoja, kansioita ja luetteloita myöntäminen vain ryhmien tai yksilöiden, jota haluat käyttää.</span><span class="sxs-lookup"><span data-stu-id="be13a-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="be13a-104">SharePoint-oikeudet periytyvät hierarkiassa ylempänä.</span><span class="sxs-lookup"><span data-stu-id="be13a-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="be13a-105">Joten tiedosto perii käyttöoikeudet sen kansion, jotka perivät käyttöoikeutensa kirjastosta, jotka perivät käyttöoikeutensa sivustosta.</span><span class="sxs-lookup"><span data-stu-id="be13a-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="be13a-106">Voit jakaa ylemmällä tasolla (esimerkiksi jakamalla koko sivuston) ja sitten keskeytettäessä periytymistä, jos et halua jakaa kaikkia sivuston.</span><span class="sxs-lookup"><span data-stu-id="be13a-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="be13a-107">Kuitenkin tämä ei ole suositeltavaa, koska se tekee ylläpito oikeudet enemmän monimutkaista ja sekavaa tulevaisuudessa.</span><span class="sxs-lookup"><span data-stu-id="be13a-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="be13a-108">Tässä on mitä voi tehdä, sen sijaan:</span><span class="sxs-lookup"><span data-stu-id="be13a-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="be13a-109">Jos esimerkiksi haluat jakaa kaikkien paitsi yhden tiedoston, kansion sisällön, siirtää tiedoston paikkaan, joka ei ole jaettu.</span><span class="sxs-lookup"><span data-stu-id="be13a-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="be13a-110">Jos kansiossa on kaksi alikansiot ja haluat jakaa ryhmiin A ja B yksi alikansio ja sallia ainoastaan ryhmän A pääsyn toiseen alikansioon, ylemmän tason kansion jakaminen ryhmän A ja lisätä ryhmän B ensimmäisen alikansion.</span><span class="sxs-lookup"><span data-stu-id="be13a-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="be13a-111">Tiedoston tai kansion jakamisen lopettaminen</span><span class="sxs-lookup"><span data-stu-id="be13a-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

