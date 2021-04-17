---
title: Omistaja ei voi luoda alikansiota Outlookin avulla
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836132"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="e4bc0-102">Omistaja ei voi luoda alikansiota Outlookin avulla</span><span class="sxs-lookup"><span data-stu-id="e4bc0-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="e4bc0-103">**Alikansioiden luomisessa Outlookissa on meneillään ongelma, jossa yleisen kansion omistajat luovat alikansioita. Ongelma korjataan pian.**</span><span class="sxs-lookup"><span data-stu-id="e4bc0-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="e4bc0-104">Sillä välin voit käyttää yhtä seuraavista vaihtoehtoista tavoista:</span><span class="sxs-lookup"><span data-stu-id="e4bc0-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="e4bc0-105">Käytä Outlook for MACia alikansion luomiseen, koska ongelma vaikuttaa vain Outlookin työpöytäversioihin (kaikki versiot)</span><span class="sxs-lookup"><span data-stu-id="e4bc0-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="e4bc0-106">Järjestelmänvalvojan on luotava alikansio EXO Shellin tai EAC:n avulla</span><span class="sxs-lookup"><span data-stu-id="e4bc0-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="e4bc0-107">Käyttäjän DefaultPublicFolderMailbox/EffectivePublicFolderMailbox-kansion muuttaminen muuhun kuin kansion sisältöpostilaatikkoon, joka aiheuttaa ongelman</span><span class="sxs-lookup"><span data-stu-id="e4bc0-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="e4bc0-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="e4bc0-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="e4bc0-109">Odota tunti, käynnistä Outlook-asiakasohjelma uudelleen</span><span class="sxs-lookup"><span data-stu-id="e4bc0-109">Wait for an hour, restart outlook client</span></span>