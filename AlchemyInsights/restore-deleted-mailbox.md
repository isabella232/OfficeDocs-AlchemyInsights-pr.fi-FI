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
ms.openlocfilehash: 284024bdf9728e8463fe69ef9c9c2695035faf2f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511361"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="d7367-102">Poistetun postilaatikon palauttaminen</span><span class="sxs-lookup"><span data-stu-id="d7367-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="d7367-103">Kun käyttäjä menettää Exchange Online -käyttöoikeuden, hänen postilaatikkonsa säilytetään 30 päivän ajan ja se voidaan palauttaa yksinkertaisesti määrittämällä käyttöoikeus uudelleen käyttäjälle.</span><span class="sxs-lookup"><span data-stu-id="d7367-103">When a user loses an Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
 <span data-ttu-id="d7367-104">*Tämä toimii vain 30 päivän kuluessa.*</span><span class="sxs-lookup"><span data-stu-id="d7367-104">*This will work only within 30 days.*</span></span>  
  
1. <span data-ttu-id="d7367-105">Siirry Microsoft 365 -hallintakeskuksessa **Käyttäjät** \> **aktiiviset käyttäjät -sivulle.**</span><span class="sxs-lookup"><span data-stu-id="d7367-105">In the Microsoft 365 admin center, go to the **Users** \> **Active users** page.</span></span> <span data-ttu-id="d7367-106">Valitse kyseinen käyttäjä.</span><span class="sxs-lookup"><span data-stu-id="d7367-106">Select the user in question.</span></span>

2. <span data-ttu-id="d7367-107">Määritä **Käyttöoikeudet ja sovellukset** -välilehdessä Exchange Online -käyttöoikeus ja valitse **Tallenna muutokset**.</span><span class="sxs-lookup"><span data-stu-id="d7367-107">On the **Licenses and Apps** tab, assign the Exchange Online license and select **Save changes**.</span></span>

<span data-ttu-id="d7367-108">Jos yrität palauttaa jaettua postilaatikkoa, se voidaan palauttaa myös 30 päivän ajan.</span><span class="sxs-lookup"><span data-stu-id="d7367-108">If you are trying to recover a Shared mailbox, it is also recoverable for 30 days.</span></span> <span data-ttu-id="d7367-109">Ne **löytyvät Käyttäjät** \> **poistetut käyttäjät**-kohdasta , jaetut postilaatikot eivät edellytä käyttöoikeutta.</span><span class="sxs-lookup"><span data-stu-id="d7367-109">You can find them under **Users** \> **Deleted users**; shared mailboxes do not require a license.</span></span> <span data-ttu-id="d7367-110">Jos huomaat, että sinun on palautettava poistettu käyttäjä, katso [käyttäjän palauttaminen](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="d7367-110">If you realize that you need to restore a deleted user, please see [Restore a user](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
  