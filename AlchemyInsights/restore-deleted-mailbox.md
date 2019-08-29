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
ms.openlocfilehash: 44b23be5e75a0669821bbeb07b0f064eeef6d021
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666369"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="5d87d-102">Poistetun postilaatikon palauttaminen</span><span class="sxs-lookup"><span data-stu-id="5d87d-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="5d87d-103">Käyttäjä menettää Exchange Online-käyttöoikeuden, kun heidän postilaatikkonsa säilytetään 30 päivää ja määrittämällä yksinkertaisesti uudelleen käyttöoikeuden käyttäjälle voidaan palauttaa.</span><span class="sxs-lookup"><span data-stu-id="5d87d-103">When a user loses an Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
 <span data-ttu-id="5d87d-104">*Tämä toimii vain 30 päivän kuluessa.*</span><span class="sxs-lookup"><span data-stu-id="5d87d-104">*This will work only within 30 days.*</span></span>  
  
1. <span data-ttu-id="5d87d-105">Siirry Microsoft-365-hallintakeskukseen **käyttäjät** \> **Aktiiviset käyttäjät** -sivulla.</span><span class="sxs-lookup"><span data-stu-id="5d87d-105">In the Microsoft 365 admin center, go to the **Users** \> **Active users** page.</span></span> <span data-ttu-id="5d87d-106">Valitse kyseinen käyttäjä.</span><span class="sxs-lookup"><span data-stu-id="5d87d-106">Select the user in question.</span></span>

2. <span data-ttu-id="5d87d-107">**Käyttöoikeudet ja Apps** -välilehdessä määrittää Exchange Online-käyttöoikeus ja valitse **Tallenna muutokset**.</span><span class="sxs-lookup"><span data-stu-id="5d87d-107">On the **Licenses and Apps** tab, assign the Exchange Online license and select **Save changes**.</span></span>

<span data-ttu-id="5d87d-108">Jos yrität palauttaa jaettu postilaatikko on myös palautettavissa oleva 30 päivän ajan.</span><span class="sxs-lookup"><span data-stu-id="5d87d-108">If you are trying to recover a Shared mailbox, it is also recoverable for 30 days.</span></span> <span data-ttu-id="5d87d-109">Voit etsiä **käyttäjät** \> **Poistetut käyttäjät**. jaettujen postilaatikoiden toiminta ei edellytä käyttöoikeutta.</span><span class="sxs-lookup"><span data-stu-id="5d87d-109">You can find them under **Users** \> **Deleted users**; shared mailboxes do not require a license.</span></span> <span data-ttu-id="5d87d-110">Jos huomaat, että sinun täytyy palauttaa poistetun käyttäjä-kohdassa [Palauta käyttäjä Office 365: ssä](https://docs.microsoft.com/office365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="5d87d-110">If you realize that you need to restore a deleted user, please see [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user).</span></span>
  