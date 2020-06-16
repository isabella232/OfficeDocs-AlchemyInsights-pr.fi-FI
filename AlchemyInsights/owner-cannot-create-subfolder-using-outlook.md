---
title: Omistaja ei voi luoda alikansiota Outlookin avulla
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/12/2020
ms.locfileid: "44748906"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="08377-102">Omistaja ei voi luoda alikansiota Outlookin avulla</span><span class="sxs-lookup"><span data-stu-id="08377-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="08377-103">**Yleisten kansioiden omistajissa on jatkuva ongelma, joka luo alikansioita Outlookin avulla. Ongelma korjataan pian.**</span><span class="sxs-lookup"><span data-stu-id="08377-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="08377-104">Käytä samalla jotakin seuraavista kiertotavoista:</span><span class="sxs-lookup"><span data-stu-id="08377-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="08377-105">Outlook for MAC:n avulla voit luoda alikansion, koska ongelma vaikuttaa vain Outlook työpöytäikkunoihin (kaikki versiot)</span><span class="sxs-lookup"><span data-stu-id="08377-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="08377-106">Hankkia admin aiheuttaa subfolder kohteleva EXO Hylsy eli EAC</span><span class="sxs-lookup"><span data-stu-id="08377-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="08377-107">Käyttäjän DefaultPublicFolderMailbox/EffectivePublicFolderMailbox-kansion muuttaminen muuhun postilaatikkoon kuin ongelman aiheuttavan kansion sisältöpostilaatikkoon</span><span class="sxs-lookup"><span data-stu-id="08377-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="08377-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="08377-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="08377-109">Odota tunti, käynnistä Outlook-asiakasohjelma uudelleen</span><span class="sxs-lookup"><span data-stu-id="08377-109">Wait for an hour, restart outlook client</span></span>