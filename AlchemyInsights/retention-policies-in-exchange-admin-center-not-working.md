---
title: Exchange-hallintakeskuksen säilytyskäytännöt eivät toimi
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 3040365b9d686bcbcce60977ee9bdbbaffc70b24
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502604"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="5a324-102">Säilytyskäytännöt Exchange-hallintakeskuksessa</span><span class="sxs-lookup"><span data-stu-id="5a324-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="5a324-103">**Numero:** Exchange-hallintakeskuksen äskettäin luodut tai päivitetyt säilytyskäytännöt eivät koske postilaatikoita tai kohteita ei siirretä arkistopostilaatikkoon tai poisteta.</span><span class="sxs-lookup"><span data-stu-id="5a324-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="5a324-104">**Perussyitä:**</span><span class="sxs-lookup"><span data-stu-id="5a324-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="5a324-105">Tämä voi johtua siitä, että **hallitun kansion avustaja** ei ole käsitellyt käyttäjän postilaatikkoa.</span><span class="sxs-lookup"><span data-stu-id="5a324-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="5a324-106">Hallitun kansion hallinta yrittää käsitellä pilvipohjaisen organisaation jokaista postilaatikkoa seitsemän päivän välein.</span><span class="sxs-lookup"><span data-stu-id="5a324-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="5a324-107">Jos muutat säilytystunnistetta tai käytät postilaatikkoon eri säilytyskäytäntöä, voit odottaa, kunnes hallittu kansioavustin käsittelee postilaatikon, tai voit käynnistää hallitun kansion hallinnan suorittamalla Start-ManagedFolderAssistant-cmdlet-otoksen ja käynnistää tietyn postilaatikon.</span><span class="sxs-lookup"><span data-stu-id="5a324-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="5a324-108">Tämän cmdlet-esityksen suorittaminen on hyödyllistä säilytyskäytännön tai säilytystunnisteen asetusten testaamisessa tai vianmäärityksessä.</span><span class="sxs-lookup"><span data-stu-id="5a324-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="5a324-109">Lisätietoja on [ohjeaiheessa Hallitun kansion hallinnan suorittaminen](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="5a324-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="5a324-110">**Ratkaisu:** Käynnistä tietyn postilaatikon hallitun kansion hallintaohjelma suorittamalla seuraava komento:</span><span class="sxs-lookup"><span data-stu-id="5a324-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="5a324-111">Näin voi käydä myös, jos **RetentionHold** on otettu **käyttöön** postilaatikossa.</span><span class="sxs-lookup"><span data-stu-id="5a324-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="5a324-112">Jos postilaatikko on sijoitettu Säilytyspalvelun säilyttämiseen, postilaatikon säilytyskäytäntöä ei käsitellä kyseisenä aikana.</span><span class="sxs-lookup"><span data-stu-id="5a324-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="5a324-113">Lisätietoja RetentionHold-asetuksesta on kohdassa [Postilaatikon säilytyspito](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="5a324-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="5a324-114">**Ratkaisu:**</span><span class="sxs-lookup"><span data-stu-id="5a324-114">**Solution:**</span></span>
    
  - <span data-ttu-id="5a324-115">Tarkista [exo powershellin](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)postilaatikon RetentionHold-asetuksen tila:</span><span class="sxs-lookup"><span data-stu-id="5a324-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="5a324-116">Poista RetentionHold **käytöstä** tietyssä postilaatikossa suorittamalla seuraava komento:</span><span class="sxs-lookup"><span data-stu-id="5a324-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="5a324-117">Suorita nyt hallitun kansion hallintaohjelma uudelleen:</span><span class="sxs-lookup"><span data-stu-id="5a324-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="5a324-118">**Huomautus:** Jos postilaatikon koko on alle 10 megatavua, hallitun kansion hallinta ei käsittele postilaatikkoa automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="5a324-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="5a324-119">Lisätietoja Exchange-hallintakeskuksen säilytyskäytännöistä on seuraavissa ohjeissa:</span><span class="sxs-lookup"><span data-stu-id="5a324-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="5a324-120">Säilytystunnisteet ja säilytyskäytännöt</span><span class="sxs-lookup"><span data-stu-id="5a324-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="5a324-121">Säilytyskäytännön käyttäminen postilaatikoissa</span><span class="sxs-lookup"><span data-stu-id="5a324-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="5a324-122">Säilytystunnisteiden lisääminen tai poistaminen</span><span class="sxs-lookup"><span data-stu-id="5a324-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="5a324-123">Postilaatikkoon sijoitetun pitoon asetetun pidon tyypin tunnistaminen</span><span class="sxs-lookup"><span data-stu-id="5a324-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
