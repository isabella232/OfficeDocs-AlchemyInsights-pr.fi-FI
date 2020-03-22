---
title: Yleisiä kansioita ei voi käyttää
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
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891746"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="10611-102">Outlook ei voi muodostaa yhteyttä yleisiin kansioihin</span><span class="sxs-lookup"><span data-stu-id="10611-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="10611-103">Jos yleisen kansion käyttö ei toimi joillekin käyttäjille, kokeile seuraavaa:</span><span class="sxs-lookup"><span data-stu-id="10611-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="10611-104">Muodosta yhteys EXO PowerShelliin ja määritä ongelmakäyttäjätilin DefaultPublicFolderMailbox-parametri vastaamaan toimivan käyttäjätilin parametria.</span><span class="sxs-lookup"><span data-stu-id="10611-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="10611-105">Esimerkki:</span><span class="sxs-lookup"><span data-stu-id="10611-105">Example:</span></span>

<span data-ttu-id="10611-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox (OletuskansioPostilaatikko),EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="10611-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="10611-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox-arvo \<edellisestä komennosta></span><span class="sxs-lookup"><span data-stu-id="10611-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="10611-108">Odota vähintään tunti, jotta muutos tulee voimaan.</span><span class="sxs-lookup"><span data-stu-id="10611-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="10611-109">Jos ongelma ei ratko, toimi [seuraavasti](https://aka.ms/pfcte) yleisen kansion käyttöongelmien vianmäärityksessä Outlookin avulla.</span><span class="sxs-lookup"><span data-stu-id="10611-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>