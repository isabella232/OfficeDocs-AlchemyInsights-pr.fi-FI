---
title: Lähetä sähkö postia käyttävänä Public-kansiona EXO-sovelluksessa
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
- "1956"
- "3500007"
ms.openlocfilehash: ed62c6d7db0ae532f806ce4fdc48f42623bcd545
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/13/2020
ms.locfileid: "48461842"
---
# <a name="sendas-mail-enabled-public-folder"></a><span data-ttu-id="0da13-102">Sähkö postin käytössä olevan julkisen kansion SendAs-toiminto</span><span class="sxs-lookup"><span data-stu-id="0da13-102">SendAs Mail Enabled Public Folder</span></span>

<span data-ttu-id="0da13-103">Seuraava esimerkki määrittää sähkö postia käyttävän yleisen kansion NewPF1-käyttö oikeudet käyttäjälle Jason.</span><span class="sxs-lookup"><span data-stu-id="0da13-103">The following example assigns "Send As" permissions for the mail-enabled public folder NewPF1 to the user Jason.</span></span>

<span data-ttu-id="0da13-104">Add-RecipientPermission-Identity ' NewPF1 '-trustee "Jason"-AccessRights "SendAs"</span><span class="sxs-lookup"><span data-stu-id="0da13-104">Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'</span></span>

<span data-ttu-id="0da13-105">Yksityiskohtaisia syntaksi-ja parametri tietoja on kohdassa [sähkö postia käyttävien julkisten kansioiden määrittäminen "Lähetä nimellä"-tai "Lähetä puolesta"-käyttö oikeudet](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span><span class="sxs-lookup"><span data-stu-id="0da13-105">For detailed syntax and parameter information see [Assign "Send As" or "Send on Behalf" permissions for mail-enabled public folders](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span></span>

