---
title: Hosted Voicemailin käyttöönotto
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/09/2020
ms.locfileid: "49678001"
---
# <a name="how-to-enable-hosted-voicemail"></a><span data-ttu-id="b14ff-102">Hosted Voicemailin käyttöönotto</span><span class="sxs-lookup"><span data-stu-id="b14ff-102">How to enable Hosted Voicemail</span></span>

<span data-ttu-id="b14ff-103">Jos haluat ottaa vasta ajan käyttöön, **Hostedvoicemail** -asetuksena on oltava $TRUE.</span><span class="sxs-lookup"><span data-stu-id="b14ff-103">To enable Voicemail, **HostedVoicemail** must be set to $true.</span></span>

<span data-ttu-id="b14ff-104">**Hostedvoicemail** -ominaisuus käyttäjän etäpowershellin (RPS) avulla.</span><span class="sxs-lookup"><span data-stu-id="b14ff-104">The **HostedVoicemail** property on the user using Remote PowerShell (RPS).</span></span>

<span data-ttu-id="b14ff-105">Lisä tietoja yhteyden muodostamisesta RPS-palveluun on [Microsoft teamsin PowerShellin yleiskatsaus](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) -kohdassa, jossa on lisä tietoja yhteyden MUODOSTAMISESTA RPS-palveluun.</span><span class="sxs-lookup"><span data-stu-id="b14ff-105">For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.</span></span>

1. <span data-ttu-id="b14ff-106">Teamsin järjestelmänvalvojan tulee olla kirjautuneena teamsin PowerShell-etäpalvelimeen.</span><span class="sxs-lookup"><span data-stu-id="b14ff-106">The Teams Admin should be logged into Remote PowerShell for Teams.</span></span>
1. <span data-ttu-id="b14ff-107">PowerShell-kehotteesta teamsin järjestelmänvalvoja voi suorittaa **joukko-csuser user@contoso.com-Hostedvoicemailin $True** , jossa SIP URI on kyseisessä käyttäjä.</span><span class="sxs-lookup"><span data-stu-id="b14ff-107">From PowerShell prompt the Teams Admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.</span></span>

> [!NOTE]
> <span data-ttu-id="b14ff-108">Käytäntöjen muutokset voivat kestää jopa 24 tuntia, ennen kuin ne replikoidaan.</span><span class="sxs-lookup"><span data-stu-id="b14ff-108">Changes to policies can take up to 24 hours to replicate.</span></span>