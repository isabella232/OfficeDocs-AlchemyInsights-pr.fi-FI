---
title: Yleisten kansioiden käyttö ei onnistu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959492"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="34f54-102">Outlook ei voi muodostaa yhteyttä julkisiin kansioihin</span><span class="sxs-lookup"><span data-stu-id="34f54-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="34f54-103">Jos yleinen kansio-käyttö ei toimi muutamilla käyttäjillä, kokeile seuraavia:</span><span class="sxs-lookup"><span data-stu-id="34f54-103">If public folder access isn't working for few users, try the following:</span></span>

<span data-ttu-id="34f54-104">Muodosta yhteys EXO PowerShelliin ja määritä Defaultpublicfolderposti laatikko ongelman käyttäjä tilille vastaamaan yhtä työn käyttäjä tilistä.</span><span class="sxs-lookup"><span data-stu-id="34f54-104">Connect to EXO PowerShell, and configure the DefaultPublicFolderMailbox on the problem user account to match one on a working user account.</span></span>

<span data-ttu-id="34f54-105">Esimerkki:</span><span class="sxs-lookup"><span data-stu-id="34f54-105">Example:</span></span>

<span data-ttu-id="34f54-106">Hanki posti laatikon Työkäyttäjä | FT Defaultpublicfolderposti laatikko, Effectivepublicfolderposti laatikko</span><span class="sxs-lookup"><span data-stu-id="34f54-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="34f54-107">Set-posti laatikko ProblemUser-Defaultpublicfolderposti laatikon \<arvo edellisestä komennosta></span><span class="sxs-lookup"><span data-stu-id="34f54-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="34f54-108">Odota vähintään yksi tunti, jotta muutos tulee voimaan.</span><span class="sxs-lookup"><span data-stu-id="34f54-108">Wait at least one hour for the change to take effect.</span></span>