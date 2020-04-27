---
title: Postilaatikon automaattisten vastausten määrittäminen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 4ffe8d77dad7db5fd5806fe879cf4934e5ca7c4a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2020
ms.locfileid: "43788879"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="f550c-102">Käyttäjän postilaatikon automaattisten vastausten määrittäminen</span><span class="sxs-lookup"><span data-stu-id="f550c-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="f550c-103">**Menetelmä 1**</span><span class="sxs-lookup"><span data-stu-id="f550c-103">**Method 1**</span></span>

1. <span data-ttu-id="f550c-104">Kirjaudu sisään Microsoft 365 -portaaliin.</span><span class="sxs-lookup"><span data-stu-id="f550c-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="f550c-105">Siirry kohtaan **Käyttäjät > Aktiiviset käyttäjät** (tai **Ryhmät > Jaetut postilaatikot**, jos määrität jaetun postilaatikon).</span><span class="sxs-lookup"><span data-stu-id="f550c-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="f550c-106">Valitse käyttäjä, jolla on Microsoft Exchange -postilaatikko.</span><span class="sxs-lookup"><span data-stu-id="f550c-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="f550c-107">Siirry oikealla olevassa pikaikkunavalikossa kohtaan **Sähköpostiasetukset > Automaattiset vastaukset** (jos kyseessä on jaettu postilaatikko, valitse pikaikkunavalikossa **Automaattiset vastaukset**).</span><span class="sxs-lookup"><span data-stu-id="f550c-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="f550c-108">**Menetelmä 2**</span><span class="sxs-lookup"><span data-stu-id="f550c-108">**Method 2**</span></span>

1. <span data-ttu-id="f550c-109">Kirjaudu sisään Microsoft 365 -hallintaportaaliin järjestelmänvalvojan tunnistetiedoilla.</span><span class="sxs-lookup"><span data-stu-id="f550c-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="f550c-110">Laajenna **Hallintakeskukset** ja valitse sitten **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="f550c-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="f550c-111">Valitse oikeassa yläkulmassa oleva kuva, valitse **Toinen käyttäjä** ja valitse sitten käyttäjäpostilaatikko, jonka haluat muuttaa.</span><span class="sxs-lookup"><span data-stu-id="f550c-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="f550c-112">Valitse vasemmalla puolella **Asetukset**, valitse **Järjestä sähköposti** ja valitse sitten **Automaattiset vastaukset.**</span><span class="sxs-lookup"><span data-stu-id="f550c-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="f550c-113">**Menetelmä 3**</span><span class="sxs-lookup"><span data-stu-id="f550c-113">**Method 3**</span></span>

<span data-ttu-id="f550c-114">Suorita seuraava cmdlet-komento Exchange Online PowerShellissä:</span><span class="sxs-lookup"><span data-stu-id="f550c-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="f550c-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="f550c-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="f550c-116">Lisätietoja tästä cmdlet-komennosta on kohdassa [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="f550c-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
