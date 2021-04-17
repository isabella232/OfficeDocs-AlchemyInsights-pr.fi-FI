---
title: Julkisten kansioiden käyttö ei ole käytettävissä
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819509"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="9661d-102">Outlook ei voi muodostaa yhteyttä yleisiin kansioihin</span><span class="sxs-lookup"><span data-stu-id="9661d-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="9661d-103">Jos yleinen kansion käyttö ei toimi joillakin käyttäjillä, kokeile seuraavaa:</span><span class="sxs-lookup"><span data-stu-id="9661d-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="9661d-104">Muodosta yhteys EXO PowerShelliin ja määritä ongelmakäyttäjätilin DefaultPublicFolderMailbox-parametri vastaamaan toimivan käyttäjätilin parametria.</span><span class="sxs-lookup"><span data-stu-id="9661d-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="9661d-105">Esimerkki:</span><span class="sxs-lookup"><span data-stu-id="9661d-105">Example:</span></span>

<span data-ttu-id="9661d-106">Get-Mailbox WorkingUser-| ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="9661d-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="9661d-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="9661d-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="9661d-108">Odota vähintään yksi tunti, jotta muutos tulee voimaan.</span><span class="sxs-lookup"><span data-stu-id="9661d-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="9661d-109">Jos ongelma ei muutu, noudata [näitä ohjeita](https://aka.ms/pfcte) yleisen kansion käytön ongelmien vianmääritykseen Outlookin avulla.</span><span class="sxs-lookup"><span data-stu-id="9661d-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="9661d-110">**Voit määrittää, k voivatko käyttäjät käyttää julkisia kansioita Outlookin avulla:**</span><span class="sxs-lookup"><span data-stu-id="9661d-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="9661d-111">Käytä Set-CASMailbox <mailboxname> -PublicFolderClientAccess -$true tai $false</span><span class="sxs-lookup"><span data-stu-id="9661d-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="9661d-112">$true: Salli käyttäjien käyttää julkisia kansioita Outlookissa</span><span class="sxs-lookup"><span data-stu-id="9661d-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="9661d-113">$false: Estä käyttäjien pääsy Yleisiin kansioihin Outlookissa.</span><span class="sxs-lookup"><span data-stu-id="9661d-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="9661d-114">Tämä on oletusarvo.</span><span class="sxs-lookup"><span data-stu-id="9661d-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="9661d-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="9661d-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="9661d-116">**Huomautus** Tämä toimenpide voi hallita yhteyksiä vain Outlookin työpöytäsovelluksella Windows-asiakassovellohjelmia varten.</span><span class="sxs-lookup"><span data-stu-id="9661d-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="9661d-117">Käyttäjä voi edelleen käyttää julkisia kansioita OWA:n tai Outlook for Macin avulla.</span><span class="sxs-lookup"><span data-stu-id="9661d-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="9661d-118">Lisätietoja on kohdassa [Valvotuille yhteyksille Outlookin](https://aka.ms/controlpf)yleisiin kansioihin -tuen ilmoittaminen.</span><span class="sxs-lookup"><span data-stu-id="9661d-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>