---
title: 1336 RecoverableItems-kansio on täynnä
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 4f0cba480fcc05114abd8f370b84e9a37e5f2804
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510749"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="5c2c8-102">Palautettavat-kansio on täynnä</span><span class="sxs-lookup"><span data-stu-id="5c2c8-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="5c2c8-103">Exchange Online -postilaatikoissa Palautettavat-kansion oletustallennusrajoitus on 30 Gigatavua.</span><span class="sxs-lookup"><span data-stu-id="5c2c8-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="5c2c8-104">Palautettavat-kansion tallennusrajoitus nostetaan automaattisesti 100 gigatavuun, jos postilaatikko sijoitetaan oikeustoimiin pitoon, eDiscovery Holdiin tai säilytyskäytäntöön.</span><span class="sxs-lookup"><span data-stu-id="5c2c8-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="5c2c8-105">Kun Palautettavat-kansio saavuttaa tallennusrajan, tämä vaikuttaa postilaatikkotoimintoon seuraavilla tavoilla:</span><span class="sxs-lookup"><span data-stu-id="5c2c8-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="5c2c8-106">Käyttäjä ei voi poistaa kohteita postilaatikosta.</span><span class="sxs-lookup"><span data-stu-id="5c2c8-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="5c2c8-107">Hallitun kansion hallinta ei voi poistaa kohteita säilytystunnisteen tai hallittujen kansioiden asetusten perusteella.</span><span class="sxs-lookup"><span data-stu-id="5c2c8-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="5c2c8-108">Postilaatikoissa, joiden yksittäinen kohde on otettu käyttöön tai jotka on sijoitettu pitoon, kopio-on-kirjoitussivun suojausprosessi ei voi ylläpitää käyttäjän muokkaamien kohteiden versioita.</span><span class="sxs-lookup"><span data-stu-id="5c2c8-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="5c2c8-109">Postilaatikoissa, joissa postilaatikon valvontaloki on käytössä, postilaatikon valvontalokimerkintöjä ei voi tallentaa Palautettavat-kansion Valvonta-alikansioon.</span><span class="sxs-lookup"><span data-stu-id="5c2c8-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="5c2c8-110">Jos postilaatikossa ei ole pidossa, järjestelmänvalvojat voivat `Search-Mailbox -SearchDumpsterOnly -DeleteContent` poistaa Palautettavat-kansion kohteita Exchange Online PowerShellin komennolla.</span><span class="sxs-lookup"><span data-stu-id="5c2c8-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="5c2c8-111">Lisätietoja on seuraavissa artikkeleissa:</span><span class="sxs-lookup"><span data-stu-id="5c2c8-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="5c2c8-112">Viestien etsiminen ja poistaminen</span><span class="sxs-lookup"><span data-stu-id="5c2c8-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="5c2c8-113">Haku-postilaatikko</span><span class="sxs-lookup"><span data-stu-id="5c2c8-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="5c2c8-114">Pidossa olevissa postilaatikoissa järjestelmänvalvojien on poistettava pito, ennen kuin he voivat poistaa kohteita Palautettavat-kansiosta.</span><span class="sxs-lookup"><span data-stu-id="5c2c8-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="5c2c8-115">Lisätietoja on [ohjeaiheessa Pidossa olevien pilvipohjaisten postilaatikoiden Palautettavat-kansion kohteiden poistaminen](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="5c2c8-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="5c2c8-116">Järjestelmänvalvojat voivat lisätä pidossa olevien postilaatikoiden Palautettavat-kansion tallennusrajoitusta ja määrittää postilaatikon säilytyskäytännön, joka siirtää kohteet Palautettavat-kansiosta käyttäjän arkistopostilaatikkoon.</span><span class="sxs-lookup"><span data-stu-id="5c2c8-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="5c2c8-117">Lisätietoja [on ohjeaiheessa Pidossa olevien postilaatikoiden palautettavan sisällön kiintiön suurentaminen](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="5c2c8-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
