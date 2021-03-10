---
title: Poistetun postilaatikon palauttaminen
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
ms.openlocfilehash: 14d2c9b1fe6764f5cd3a5a968586a19a03b62694
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50641515"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="efa31-102">Poistetun postilaatikon palauttaminen</span><span class="sxs-lookup"><span data-stu-id="efa31-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="efa31-103">Kun käyttäjä menettää Exchange Online -käyttöoikeuden, hänen postilaatikkoaan säilytetään 30 päivän ajan, ja se voidaan palauttaa määrittämällä käyttöoikeus uudelleen käyttäjälle.</span><span class="sxs-lookup"><span data-stu-id="efa31-103">When a user loses an Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
1. <span data-ttu-id="efa31-104">Siirry Microsoft 365 -hallintakeskuksessa  Käyttäjien \> **aktiiviset käyttäjät -sivulle.**</span><span class="sxs-lookup"><span data-stu-id="efa31-104">In the Microsoft 365 admin center, go to the **Users** \> **Active users** page.</span></span> <span data-ttu-id="efa31-105">Valitse haluamasi käyttäjä.</span><span class="sxs-lookup"><span data-stu-id="efa31-105">Select the user in question.</span></span>

2. <span data-ttu-id="efa31-106">Määritä Käyttöoikeudet **ja sovellukset -välilehdessä** Exchange Online -käyttöoikeus ja valitse **Tallenna muutokset.**</span><span class="sxs-lookup"><span data-stu-id="efa31-106">On the **Licenses and Apps** tab, assign the Exchange Online license and select **Save changes**.</span></span>

<span data-ttu-id="efa31-107">Jos yrität palauttaa jaettua postilaatikkoa tai poistettua käyttäjää, se on myös palautettavissa 30 päivän ajan.</span><span class="sxs-lookup"><span data-stu-id="efa31-107">If you are trying to recover a shared mailbox or a user that was deleted, it is also recoverable for 30 days.</span></span> <span data-ttu-id="efa31-108">Löydät ne käyttäjät poistetut **käyttäjät** \> **-kohdasta;** jaetut postilaatikot eivät edellytä käyttöoikeutta.</span><span class="sxs-lookup"><span data-stu-id="efa31-108">You can find them under **Users** \> **Deleted users**; shared mailboxes do not require a license.</span></span> <span data-ttu-id="efa31-109">Lisätietoja on [kohdassa Käyttäjän palauttaminen.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)</span><span class="sxs-lookup"><span data-stu-id="efa31-109">Please see [Restore a user](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="efa31-110">Järjestelmänvalvojat voivat tehdä sähköpostin palauttamisen käyttäjän postilaatikosta uuteen [Exchange-hallintakeskukseen.](https://techcommunity.microsoft.com/t5/exchange-team-blog/a-new-recoverableitems-experience-comes-to-exchange-online/ba-p/1505353)</span><span class="sxs-lookup"><span data-stu-id="efa31-110">Recovery of email from user's mailbox can be done by admins by going to the [new Exchange Admin Center](https://techcommunity.microsoft.com/t5/exchange-team-blog/a-new-recoverableitems-experience-comes-to-exchange-online/ba-p/1505353).</span></span>

<span data-ttu-id="efa31-111">Jos yrität palauttaa passiivista postilaatikkoa, noudata seuraavia [ohjeita.](https://docs.microsoft.com/microsoft-365/compliance/recover-an-inactive-mailbox)</span><span class="sxs-lookup"><span data-stu-id="efa31-111">Finally, if you are trying to recover an Inactive mailbox, [follow the instructions here](https://docs.microsoft.com/microsoft-365/compliance/recover-an-inactive-mailbox).</span></span>
  
