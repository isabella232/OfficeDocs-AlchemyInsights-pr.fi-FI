---
title: 1336 Recovertableitems-kansio on täynnä
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741264"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="10b3c-102">Palautettavat-kansio on täynnä</span><span class="sxs-lookup"><span data-stu-id="10b3c-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="10b3c-103">Exchange Online-posti laatikot: Palautettavat-kansion oletus tallennus tilan enimmäismäärä on 30 Giga tavua.</span><span class="sxs-lookup"><span data-stu-id="10b3c-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="10b3c-104">Palautettavat-kansion tallennus tilan enimmäismäärä kasvaa automaattisesti 100 Giga tavuun, jos posti laatikko on asetettu oikeus toimiin liittyvään pitoon, eDiscoveryn pitoon tai kun se on määritetty säilytys käytännölle.</span><span class="sxs-lookup"><span data-stu-id="10b3c-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="10b3c-105">Kun Palautettavat-kansion tallennus tila on ylittyä, posti laatikko toimintoon vaikuttavat seuraavat asiat:</span><span class="sxs-lookup"><span data-stu-id="10b3c-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="10b3c-106">Käyttäjä ei voi poistaa kohteita posti laatikosta.</span><span class="sxs-lookup"><span data-stu-id="10b3c-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="10b3c-107">Hallitun kansion avustaja ei voi poistaa kohteita säilytys tunnisteen tai hallittujen kansioiden asetusten perusteella.</span><span class="sxs-lookup"><span data-stu-id="10b3c-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="10b3c-108">Jos posti laatikoissa on otettu käyttöön yksi kohde tai ne on sijoitettu pitoon, kopio sivun suojaus prosessi ei voi ylläpitää käyttäjän muokkaamien kohteiden versioita.</span><span class="sxs-lookup"><span data-stu-id="10b3c-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="10b3c-109">Posti laatikoiden valvonta lokin merkintöjä ei voi tallentaa Palautettavat-kansion tarkastukset-alikansioon, jos posti laatikon valvonta loki on käytössä.</span><span class="sxs-lookup"><span data-stu-id="10b3c-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="10b3c-110">Jos posti laatikot eivät ole pidossa, järjestelmänvalvojat voivat `Search-Mailbox -SearchDumpsterOnly -DeleteContent` poistaa kohteita palautettavat-kansiosta käyttämällä Exchange Online PowerShellin komentoa.</span><span class="sxs-lookup"><span data-stu-id="10b3c-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="10b3c-111">Lisätietoja on seuraavissa artikkeleissa:</span><span class="sxs-lookup"><span data-stu-id="10b3c-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="10b3c-112">Viestien etsiminen ja poistaminen</span><span class="sxs-lookup"><span data-stu-id="10b3c-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="10b3c-113">Haku-posti laatikko</span><span class="sxs-lookup"><span data-stu-id="10b3c-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="10b3c-114">Jos käytössä on pidossa olevat posti laatikot, järjestelmänvalvojien on poistettava pito, ennen kuin he voivat poistaa kohteita palautettavat-kansiosta.</span><span class="sxs-lookup"><span data-stu-id="10b3c-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="10b3c-115">Lisä tietoja on Ohje aiheessa [pidossa olevien pilvipohjaisten posti laatikoiden Palautettavat-kansion kohteiden poistaminen](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="10b3c-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="10b3c-116">Jos haluat estää Palautettavat-kansion täysimääräisen tulemisen, järjestelmänvalvojat voivat suurentaa pidossa olevien posti laatikoiden Palautettavat-kansion tallennus tilan rajoitusta ja määrittää posti laatikon säilytys käytännön, joka siirtää kohteita palautettavat-kansiosta käyttäjän Arkisto posti laatikkoon.</span><span class="sxs-lookup"><span data-stu-id="10b3c-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="10b3c-117">Katso lisä tietoja [pidossa olevien posti laatikoiden palautettavat-kiintiön korottamisesta](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="10b3c-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
