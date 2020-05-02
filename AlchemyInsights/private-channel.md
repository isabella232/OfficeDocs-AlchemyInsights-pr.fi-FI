---
title: Yksityinen kanava
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005435"
---
# <a name="private-channels-in-microsoft-teams"></a><span data-ttu-id="0f7c9-102">Yksityiset kanavat Microsoft Teamsissa</span><span class="sxs-lookup"><span data-stu-id="0f7c9-102">Private channels in Microsoft Teams</span></span>

<span data-ttu-id="0f7c9-103">Yksityiset kanavat ovat microsoft Teamsin uusi ominaisuus.</span><span class="sxs-lookup"><span data-stu-id="0f7c9-103">Private channels is a new feature in Microsoft Teams.</span></span> <span data-ttu-id="0f7c9-104">Huomaa, että yksityisiä kanavia ei voi muuntaa vakiokanavista tai päinvastoin.</span><span class="sxs-lookup"><span data-stu-id="0f7c9-104">Note that private channels cannot be converted from standard channels or vice versa.</span></span>

<span data-ttu-id="0f7c9-105">Lisätietoja yksityisistä kanavista, kuten [yksityiskanavien luomisesta ja jäsenyydestä](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) sekä [yksityisestä SharePoint-sivustoista](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), on kohdassa [Microsoft Teamsin yksityiset kanavat](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span><span class="sxs-lookup"><span data-stu-id="0f7c9-105">For details about private channels, such as information on [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) and [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), see [Private channels in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span></span> 

<span data-ttu-id="0f7c9-106">**Huomautus:** Koska yksityisten kanavien viestien säilyttämisen määritystä ei vielä tueta, vuokraajat, joiden säilytyskäytännöt ovat käytössä, eivät oletusarvoisesti ota käyttöön yksityisiä kanavia.</span><span class="sxs-lookup"><span data-stu-id="0f7c9-106">**Note:** Because configuration for retention of private channel messages is not yet supported, tenants with retention policies enabled will not have private channels enabled by default.</span></span> <span data-ttu-id="0f7c9-107">Yksityiset kanavat voidaan ottaa käyttöön Teams-hallintakeskuksessa.</span><span class="sxs-lookup"><span data-stu-id="0f7c9-107">Private channels can be enabled in the Teams admin center.</span></span> <span data-ttu-id="0f7c9-108">Huomaa myös, että vaikka yksityisten kanavien viestien säilyttämistä ei tueta, yksityisissä kanavissa jaettujen tiedostojen säilyttämistä tuetaan.</span><span class="sxs-lookup"><span data-stu-id="0f7c9-108">Also, note that while retention of private channel messages is not supported, retention of files shared in private channels is supported.</span></span>

<span data-ttu-id="0f7c9-109">**Tarvitsetko uuden tiimin omistajan?**</span><span class="sxs-lookup"><span data-stu-id="0f7c9-109">**Need a new team owner?**</span></span>

<span data-ttu-id="0f7c9-110">Jos yksityinen kanavasi omistaja lähtee, voit lisätä uuden tiimin omistajan Teams Powershellin kautta.</span><span class="sxs-lookup"><span data-stu-id="0f7c9-110">If your private channel owner leaves, you can add a new team owner via Teams Powershell.</span></span>


- <span data-ttu-id="0f7c9-111">[Siirry tästä](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) asentaaKsesi Teams Powershellin.</span><span class="sxs-lookup"><span data-stu-id="0f7c9-111">Go [here](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) to install Teams Powershell.</span></span>

<span data-ttu-id="0f7c9-112">Tässä on cmdlet tarvitset:</span><span class="sxs-lookup"><span data-stu-id="0f7c9-112">Here is the cmdlet you will need:</span></span>

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

<span data-ttu-id="0f7c9-113">Lisätietoja Teams Powershellistä on kohdassa [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="0f7c9-113">For more information on Teams Powershell, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span>
