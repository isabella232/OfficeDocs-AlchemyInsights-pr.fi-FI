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
ms.openlocfilehash: fb10b792981040bdcf4661b8aff30733c2438212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720249"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="ce500-102">Palautettavat-kansio on täynnä</span><span class="sxs-lookup"><span data-stu-id="ce500-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="ce500-103">Exchange Online -postilaatikoissa Palautettavat kohteet -kansion oletustallennusrajoitus on 30 Gigatavua.</span><span class="sxs-lookup"><span data-stu-id="ce500-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="ce500-104">Palautettavat-kansion tallennusraja nostetaan automaattisesti 100 Gigatavuun, jos postilaatikko asetetaan Oikeustoimiin liittyvään pitoon, eDiscovery-pitoon tai säilytyskäytäntöön.</span><span class="sxs-lookup"><span data-stu-id="ce500-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="ce500-105">Kun Palautettavat-kansio saavuttaa tallennusrajoituksen, postilaatikkotoiminto vaikuttaa seuraaviin tapoihin:</span><span class="sxs-lookup"><span data-stu-id="ce500-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="ce500-106">Käyttäjä ei voi poistaa postilaatikon kohteita.</span><span class="sxs-lookup"><span data-stu-id="ce500-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="ce500-107">Hallitun kansion avustaja ei voi poistaa kohteita säilytystunnisteen tai hallitun kansion asetusten perusteella.</span><span class="sxs-lookup"><span data-stu-id="ce500-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="ce500-108">Postilaatikoissa, joiden yksittäisen kohteen palautus on käytössä tai jotka on sijoitettu pitoon, kopioinnin sivun suojausprosessi ei voi ylläpitää käyttäjän muokkaamien kohteiden versioita.</span><span class="sxs-lookup"><span data-stu-id="ce500-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="ce500-109">Postilaatikoissa, joissa postilaatikon valvontaloki on käytössä, ei voi tallentaa postilaatikon valvontalokin merkintöjä Palautettavat-kansion Valvonta-alikansioon.</span><span class="sxs-lookup"><span data-stu-id="ce500-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="ce500-110">Jos postilaatikot eivät ole pidossa, järjestelmänvalvojat voivat poistaa palautettavat kohteet -kansion kohteiden poistamisesta Exchange Online PowerShellin `Search-Mailbox -SearchDumpsterOnly -DeleteContent` komennolla.</span><span class="sxs-lookup"><span data-stu-id="ce500-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="ce500-111">Lisätietoja on seuraavissa artikkeleissa:</span><span class="sxs-lookup"><span data-stu-id="ce500-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="ce500-112">Viestien etsiminen ja poistaminen</span><span class="sxs-lookup"><span data-stu-id="ce500-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="ce500-113">Haku-postilaatikko</span><span class="sxs-lookup"><span data-stu-id="ce500-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="ce500-114">Pidossa olevien postilaatikoiden järjestelmänvalvojien on poistettava pito, ennen kuin he voivat poistaa kohteita Palautettavat-kansiosta.</span><span class="sxs-lookup"><span data-stu-id="ce500-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="ce500-115">Lisätietoja on [ohjeaiheessa Pilvipohjaisten postilaatikoiden Palautettavat-kansion kohteiden poistaminen pidossa](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="ce500-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="ce500-116">Järjestelmänvalvojat voivat pidentää palautettavat kohteet -kansion täyttämistä lisäämättä pitopostilaatikoiden Palautettavat-kansion tallennusrajoitusta ja määrittää postilaatikon säilytyskäytännön, joka siirtää kohteet Palautettavat-kansiosta käyttäjän arkistopostilaatikkoon.</span><span class="sxs-lookup"><span data-stu-id="ce500-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="ce500-117">Katso [Pitopostilaatikoiden Palautettavat-kiintiön suurentaminen](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="ce500-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
