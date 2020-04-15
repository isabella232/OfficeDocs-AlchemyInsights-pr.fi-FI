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
ms.openlocfilehash: aeeb2e1e76fe602d2767b422797452fd1155fdd5
ms.sourcegitcommit: fdfd41c2bfb2d45003b3906e6469377384a91cb5
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2020
ms.locfileid: "43509491"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="b50a4-102">Käyttäjän postilaatikon automaattisten vastausten määrittäminen</span><span class="sxs-lookup"><span data-stu-id="b50a4-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="b50a4-103">**Menetelmä 1**</span><span class="sxs-lookup"><span data-stu-id="b50a4-103">**Method 1**</span></span>

1. <span data-ttu-id="b50a4-104">Kirjaudu sisään Office 365 -portaaliin.</span><span class="sxs-lookup"><span data-stu-id="b50a4-104">Sign in to the Office 365 portal.</span></span>

2. <span data-ttu-id="b50a4-105">Siirry kohtaan **Käyttäjät > Aktiiviset käyttäjät** (tai **Ryhmät > Jaetut postilaatikot**, jos määrität jaetun postilaatikon).</span><span class="sxs-lookup"><span data-stu-id="b50a4-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="b50a4-106">Valitse käyttäjä, jolla on Microsoft Exchange -postilaatikko.</span><span class="sxs-lookup"><span data-stu-id="b50a4-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="b50a4-107">Siirry oikealla olevassa pikaikkunavalikossa kohtaan **Sähköpostiasetukset > Automaattiset vastaukset** (jos kyseessä on jaettu postilaatikko, valitse pikaikkunavalikossa **Automaattiset vastaukset**).</span><span class="sxs-lookup"><span data-stu-id="b50a4-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="b50a4-108">**Menetelmä 2**</span><span class="sxs-lookup"><span data-stu-id="b50a4-108">**Method 2**</span></span>

1. <span data-ttu-id="b50a4-109">Kirjaudu sisään Office 365 -hallintaportaaliin järjestelmänvalvojan tunnistetiedoilla.</span><span class="sxs-lookup"><span data-stu-id="b50a4-109">Sign in to the Office 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="b50a4-110">Laajenna **Hallintakeskukset** ja valitse sitten **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="b50a4-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="b50a4-111">Valitse oikeassa yläkulmassa oleva kuva, valitse **Toinen käyttäjä** ja valitse sitten käyttäjäpostilaatikko, jonka haluat muuttaa.</span><span class="sxs-lookup"><span data-stu-id="b50a4-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="b50a4-112">Valitse vasemmalla puolella **Asetukset**, valitse **Järjestä sähköposti** ja valitse sitten **Automaattiset vastaukset.**</span><span class="sxs-lookup"><span data-stu-id="b50a4-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="b50a4-113">**Menetelmä 3**</span><span class="sxs-lookup"><span data-stu-id="b50a4-113">**Method 3**</span></span>

<span data-ttu-id="b50a4-114">Suorita seuraava cmdlet-komento Exchange Online PowerShellissä:</span><span class="sxs-lookup"><span data-stu-id="b50a4-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="b50a4-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="b50a4-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="b50a4-116">Lisätietoja tästä cmdlet-komennosta on kohdassa [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="b50a4-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
