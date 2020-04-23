---
title: Palauta poistettu postilaatikko
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "360"
- "3500005"
search.appverid:
- MOE150
- MED150
- MBS150
ms.assetid: e6112a76-bbb6-4c22-b2e6-690b004d92d4
ms.openlocfilehash: 18e56305b60469422a154ffa1b097c238baaae16
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764653"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="caa5f-102">Poistetun postilaatikon palauttaminen</span><span class="sxs-lookup"><span data-stu-id="caa5f-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="caa5f-103">Kun käyttäjä menettää Exchange Online -käyttöoikeuden, hänen postilaatikkonsa säilytetään 30 päivän ajan, ja se voidaan palauttaa määrittämällä käyttöoikeus käyttäjälle uudelleen.</span><span class="sxs-lookup"><span data-stu-id="caa5f-103">When a user loses an Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
 <span data-ttu-id="caa5f-104">*Tämä toimii vain 30 päivän kuluessa.*</span><span class="sxs-lookup"><span data-stu-id="caa5f-104">*This will work only within 30 days.*</span></span>  
  
1. <span data-ttu-id="caa5f-105">Siirry Microsoft 365 -hallintakeskuksessa **Käyttäjät** \> **aktiiviset käyttäjät -sivulle.**</span><span class="sxs-lookup"><span data-stu-id="caa5f-105">In the Microsoft 365 admin center, go to the **Users** \> **Active users** page.</span></span> <span data-ttu-id="caa5f-106">Valitse kyseinen käyttäjä.</span><span class="sxs-lookup"><span data-stu-id="caa5f-106">Select the user in question.</span></span>

2. <span data-ttu-id="caa5f-107">Määritä **Käyttöoikeudet ja sovellukset -välilehdessä** Exchange Online -käyttöoikeus ja valitse **Tallenna muutokset**.</span><span class="sxs-lookup"><span data-stu-id="caa5f-107">On the **Licenses and Apps** tab, assign the Exchange Online license and select **Save changes**.</span></span>

<span data-ttu-id="caa5f-108">Jos yrität palauttaa jaettua postilaatikkoa, se on myös palautettavissa 30 päivän ajan.</span><span class="sxs-lookup"><span data-stu-id="caa5f-108">If you are trying to recover a Shared mailbox, it is also recoverable for 30 days.</span></span> <span data-ttu-id="caa5f-109">Löydät ne **Käyttäjät** \> **poistetut käyttäjät**; jaetut postilaatikot eivät vaadi käyttöoikeutta.</span><span class="sxs-lookup"><span data-stu-id="caa5f-109">You can find them under **Users** \> **Deleted users**; shared mailboxes do not require a license.</span></span> <span data-ttu-id="caa5f-110">Jos huomaat, että poistettu käyttäjä on palautettava, katso [lisätietoja ohjeaiheesta Käyttäjän palauttaminen](https://docs.microsoft.com/office365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="caa5f-110">If you realize that you need to restore a deleted user, please see [Restore a user](https://docs.microsoft.com/office365/admin/add-users/restore-user).</span></span>
  