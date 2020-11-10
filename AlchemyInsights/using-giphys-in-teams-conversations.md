---
title: Giphys-käyttö teamsin keskusteluissa
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982458"
---
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="37f5c-102">Giphys-käyttö teamsin keskusteluissa</span><span class="sxs-lookup"><span data-stu-id="37f5c-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="37f5c-103">Giphys-käyttö oikeus teamsin keskustelussa on oletusarvoisesti käytössä.</span><span class="sxs-lookup"><span data-stu-id="37f5c-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="37f5c-104">Järjestelmänvalvojana voit hallita sitä, voivatko käyttäjät käyttää käyttäjiä asettamalla [viestintä käytäntöä](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) ja **varmistamalla, että** **keskustelujen käyttö** on käytössä.</span><span class="sxs-lookup"><span data-stu-id="37f5c-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="37f5c-105">Jos GIF ei toimi oikein teamsin keskusteluissa, tarkista seuraavat asiat:</span><span class="sxs-lookup"><span data-stu-id="37f5c-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="37f5c-106">[Viestintä käytäntöjen](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) on sallittava giphys.</span><span class="sxs-lookup"><span data-stu-id="37f5c-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="37f5c-107">Varmentamaan PowerShell-cmdlet-komennolla:</span><span class="sxs-lookup"><span data-stu-id="37f5c-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="37f5c-108">Varmista, että voit [hallita Teamsia PowerShellin avulla](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="37f5c-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="37f5c-109">Suorita PowerShell-komento [Get-CsTeamsMessagingPolicy-Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) ja varmista, että **Allowgiphy** -asetuksena on **True**.</span><span class="sxs-lookup"><span data-stu-id="37f5c-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="37f5c-110">Jos **Allowgiphy-parametrin** arvo on **false** , suorita seuraava PowerShell [-komento joukko-CsTeamsMessagingPolicy-Identity Global-allowgiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="37f5c-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="37f5c-111">Jos haluat käyttää Giphy-URL-osoitetta, [valinnaisten yhdistettyjen kokemusten](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) on oltava käytössä.</span><span class="sxs-lookup"><span data-stu-id="37f5c-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="37f5c-112">Jos sinulla on useita teamsin viestintä käytäntöjä, voit määrittää käyttäjälle, jolle ongelma on määritetty, PowerShell [-komennolla Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Valitse TeamsMessagingPolicy.</span><span class="sxs-lookup"><span data-stu-id="37f5c-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>
