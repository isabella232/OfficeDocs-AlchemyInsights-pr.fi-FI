---
title: Omistaja ei voi luoda alikansiota Outlookin avulla
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665715"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="bf4c6-102">Omistaja ei voi luoda alikansiota Outlookin avulla</span><span class="sxs-lookup"><span data-stu-id="bf4c6-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="bf4c6-103">**Julkisten kansioiden omistajien käytössä on jatkuva ongelma, joka luo alikansioita Outlookin avulla. Ongelma korjataan pian.**</span><span class="sxs-lookup"><span data-stu-id="bf4c6-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="bf4c6-104">Käytä samalla jotakin seuraavista vaihtoehtoisista menetelmistä:</span><span class="sxs-lookup"><span data-stu-id="bf4c6-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="bf4c6-105">Alikansion luominen Outlook for Macin avulla ongelma koskee vain Outlookin Työpöytä version ikkunoita (kaikki versiot)</span><span class="sxs-lookup"><span data-stu-id="bf4c6-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="bf4c6-106">Järjestelmänvalvojan on luotava alikansio EXO Shell-tai EAC-toiminnon avulla</span><span class="sxs-lookup"><span data-stu-id="bf4c6-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="bf4c6-107">Käyttäjän oletus kansio posti laatikon/Effectivepublic-posti laatikon muuttaminen muulle posti laatikolle kuin ongelman aiheuttavan kansion sisältö posti laatikko</span><span class="sxs-lookup"><span data-stu-id="bf4c6-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="bf4c6-108">*Asetukset-posti laatikon Käyttäjä1:n Defaoletus Publikansiposti laatikko PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="bf4c6-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="bf4c6-109">Odota tunti, Käynnistä Outlook-asiakas ohjelma uudelleen</span><span class="sxs-lookup"><span data-stu-id="bf4c6-109">Wait for an hour, restart outlook client</span></span>