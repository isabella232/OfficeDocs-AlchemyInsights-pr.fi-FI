---
title: Postilaatikon automaattisten vastausten määrittäminen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 60af581e7fe508ab9644a53873bcd551b3aacff1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820931"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="8da47-102">Käyttäjän postilaatikon automaattisten vastausten määrittäminen</span><span class="sxs-lookup"><span data-stu-id="8da47-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="8da47-103">**Menetelmä 1**</span><span class="sxs-lookup"><span data-stu-id="8da47-103">**Method 1**</span></span>

1. <span data-ttu-id="8da47-104">Kirjaudu sisään Microsoft 365 -portaaliin.</span><span class="sxs-lookup"><span data-stu-id="8da47-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="8da47-105">Siirry kohtaan **Käyttäjät > Aktiiviset käyttäjät** (tai **Ryhmät > Jaetut postilaatikot**, jos määrität jaetun postilaatikon).</span><span class="sxs-lookup"><span data-stu-id="8da47-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="8da47-106">Valitse käyttäjä, jolla on Microsoft Exchange -postilaatikko.</span><span class="sxs-lookup"><span data-stu-id="8da47-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="8da47-107">Siirry oikealla olevassa pikaikkunavalikossa kohtaan **Sähköpostiasetukset > Automaattiset vastaukset** (jos kyseessä on jaettu postilaatikko, valitse pikaikkunavalikossa **Automaattiset vastaukset**).</span><span class="sxs-lookup"><span data-stu-id="8da47-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="8da47-108">**Menetelmä 2**</span><span class="sxs-lookup"><span data-stu-id="8da47-108">**Method 2**</span></span>

1. <span data-ttu-id="8da47-109">Kirjaudu sisään Microsoft 365 -hallintaportaaliin järjestelmänvalvojan tunnistetiedoilla.</span><span class="sxs-lookup"><span data-stu-id="8da47-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="8da47-110">Laajenna **Hallintakeskukset** ja valitse sitten **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="8da47-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="8da47-111">Valitse oikeassa yläkulmassa oleva kuva, valitse **Toinen käyttäjä** ja valitse sitten käyttäjäpostilaatikko, jonka haluat muuttaa.</span><span class="sxs-lookup"><span data-stu-id="8da47-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="8da47-112">Valitse vasemmalla puolella **Asetukset**, valitse **Järjestä sähköposti** ja valitse sitten **Automaattiset vastaukset.**</span><span class="sxs-lookup"><span data-stu-id="8da47-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="8da47-113">**Menetelmä 3**</span><span class="sxs-lookup"><span data-stu-id="8da47-113">**Method 3**</span></span>

<span data-ttu-id="8da47-114">Suorita seuraava cmdlet-komento Exchange Online PowerShellissä:</span><span class="sxs-lookup"><span data-stu-id="8da47-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="8da47-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="8da47-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="8da47-116">Lisätietoja tästä cmdlet-komennosta on kohdassa [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="8da47-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
