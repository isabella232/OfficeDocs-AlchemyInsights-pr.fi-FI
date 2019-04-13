---
title: 1336 RecoverableItems kansio on täynnä
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1336
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 14d46980caf7dac90e73c34482a3aee34382fa1f
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/13/2019
ms.locfileid: "31858993"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="8b91b-102">Palautettavat kohteet-kansio on täynnä</span><span class="sxs-lookup"><span data-stu-id="8b91b-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="8b91b-103">Office 365-postilaatikot Exchange Online-palautettavat kohteet-kansio oletusarvoisesti enimmäiskoko on 30 GB.</span><span class="sxs-lookup"><span data-stu-id="8b91b-103">For Exchange Online mailboxes in Office 365, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="8b91b-104">Palautettavat kohteet-kansion enimmäiskoko on automaattisesti kasvoi 100 GB Jos postilaatikko on sijoitettu pidä oikeudenkäyntiä eDiscovery pito tai Office 365-säilytyskäytäntö on määritetty.</span><span class="sxs-lookup"><span data-stu-id="8b91b-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to an Office 365 retention policy.</span></span>

<span data-ttu-id="8b91b-105">Kun palautettavat kohteet-kansion enimmäiskoko, postilaatikko-toiminto vaikuttaa seuraavilla tavoilla:</span><span class="sxs-lookup"><span data-stu-id="8b91b-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="8b91b-106">Käyttäjä voi poistaa postilaatikon kohteita.</span><span class="sxs-lookup"><span data-stu-id="8b91b-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="8b91b-107">Hallitun kansion avustajan voi poistaa kohteita pidätys tunniste tai hallitun kansion asetusten perusteella.</span><span class="sxs-lookup"><span data-stu-id="8b91b-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="8b91b-108">Postilaatikot, jotka ovat yksittäisen kohteen palauttaminen käytössä tai ovat pidossa, copy-kirjoittaa sivulla suojauksen prosessi ei voi ylläpitää käyttäjä ryhtyy muokkaamaan kohdeversioiden.</span><span class="sxs-lookup"><span data-stu-id="8b91b-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="8b91b-109">Postilaatikot, joilla valvoa kirjaaminen on otettu käyttöön postilaatikon postilaatikko ei ole valvonnan tapahtumat voidaan tallentaa tarkastuksia palautettavat kohteet-kansion alikansioon.</span><span class="sxs-lookup"><span data-stu-id="8b91b-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="8b91b-110">Postilaatikot, jotka eivät ole estetty, järjestelmänvalvojat voivat käyttää `Search-Mailbox -SearchDumpsterOnly -DeleteContent` komento Exchange Online PowerShell poistaa kohteita palautettavat kohteet-kansiossa.</span><span class="sxs-lookup"><span data-stu-id="8b91b-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="8b91b-111">Lisätietoja on seuraavissa artikkeleissa:</span><span class="sxs-lookup"><span data-stu-id="8b91b-111">For more information, see the following topics:</span></span> 

- [<span data-ttu-id="8b91b-112">Etsi ja poista viestejä</span><span class="sxs-lookup"><span data-stu-id="8b91b-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="8b91b-113">Search-Mailbox-</span><span class="sxs-lookup"><span data-stu-id="8b91b-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="8b91b-114">Pidossa olevat postilaatikot valvojat ovat pidosta, ennen kuin he voivat palauttaa kohteet-kansiosta poistettuja kohteita.</span><span class="sxs-lookup"><span data-stu-id="8b91b-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="8b91b-115">Lisätietoja [kerrytettävissä olevan kansion pilvipohjainen postilaatikoita, pidä kohteet kohteiden poistaminen](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="8b91b-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="8b91b-116">Voit estää tulemasta koko palautettavat kohteet-kansio, järjestelmänvalvojat lisäävät kerrytettävissä oleva nimikkeiden kansiota postilaatikoita varten hallussaan ja, jossa nimikkeitä siirretään palautettavat kohteet-kansioon arkistoon käyttäjän postilaatikon säilytyskäytäntö määritetty enimmäiskoko postilaatikko.</span><span class="sxs-lookup"><span data-stu-id="8b91b-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="8b91b-117">Lisätietoja [kerrytettävissä kohteet kiintiön postilaatikoita, pidä kasvattaa](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="8b91b-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
