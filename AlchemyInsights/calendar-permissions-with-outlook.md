---
title: Kalenterin käyttöoikeudet
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862096"
---
# <a name="calendar-permissions"></a><span data-ttu-id="2d622-102">Kalenterin käyttöoikeudet</span><span class="sxs-lookup"><span data-stu-id="2d622-102">Calendar Permissions</span></span>

<span data-ttu-id="2d622-103">Käyttäjät voivat muuttaa omia kalenterioikeuksiaan Outlookin web-sivustolla tai muissa asiakkaissa, mutta järjestelmänvalvojana sinun on ehkä tutkittava myös.</span><span class="sxs-lookup"><span data-stu-id="2d622-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="2d622-104">Exchange PowerShellin cmdlet-liittimessä näytetään käyttäjän kalenterin käyttöoikeudet:</span><span class="sxs-lookup"><span data-stu-id="2d622-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="2d622-105">Lisätietoja on seuraavissa ohjeissa:</span><span class="sxs-lookup"><span data-stu-id="2d622-105">To see more information see the following:</span></span>

- [<span data-ttu-id="2d622-106">Get-MailboxFolderPermission (Get-MailboxFolderPermission) -kansion</span><span class="sxs-lookup"><span data-stu-id="2d622-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="2d622-107">Aseta mailbox-kansionroisti</span><span class="sxs-lookup"><span data-stu-id="2d622-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="2d622-108">Lisää postilaatikkokansioPermission</span><span class="sxs-lookup"><span data-stu-id="2d622-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="2d622-109">Kalenterin käyttöoikeuksia käytetään kalenterien jakamisessa, jotta saat lisätietoja Outlook-kalenterin jakamisesta, katso seuraavat artikkelit:</span><span class="sxs-lookup"><span data-stu-id="2d622-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="2d622-110">Outlook-kalenterin jakaminen muiden kanssa</span><span class="sxs-lookup"><span data-stu-id="2d622-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="2d622-111">Kalenterin jakaminen Outlookin verkkoversiossa yrityksille</span><span class="sxs-lookup"><span data-stu-id="2d622-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="2d622-112">Voit tehdä kalenterin käyttöoikeuksien vianmäärityksen [tuki- ja palautusavustajatyökalun](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) avulla.</span><span class="sxs-lookup"><span data-stu-id="2d622-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>