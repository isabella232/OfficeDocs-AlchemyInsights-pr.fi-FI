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
ms.openlocfilehash: 4d3ca121c8d22a0900f136f7f2a754dfb5b435f5
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522804"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="e1387-102">Säilytyskäytännöt Exchange-hallintakeskuksessa</span><span class="sxs-lookup"><span data-stu-id="e1387-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="e1387-103">Jos haluat meidän tarkistavan alla mainitut asetukset automaattisesti, valitse tämän sivun yläreunasta < takaisin-painike ja kirjoita sitten sen käyttäjän sähköpostiosoite, jolla on säilytyskäytäntöihin liittyviä ongelmia.</span><span class="sxs-lookup"><span data-stu-id="e1387-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="e1387-104">**Numero:** Exchange-hallintakeskuksen äskettäin luodut tai päivitetyt säilytyskäytännöt eivät koske postilaatikoita tai kohteita ei siirretä arkistopostilaatikkoon tai poisteta.</span><span class="sxs-lookup"><span data-stu-id="e1387-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="e1387-105">**Perussyitä:**</span><span class="sxs-lookup"><span data-stu-id="e1387-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="e1387-106">Tämä voi johtua siitä, että **hallitun kansion avustaja** ei ole käsitellyt käyttäjän postilaatikkoa.</span><span class="sxs-lookup"><span data-stu-id="e1387-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="e1387-107">Hallitun kansion hallinta yrittää käsitellä pilvipohjaisen organisaation jokaista postilaatikkoa seitsemän päivän välein.</span><span class="sxs-lookup"><span data-stu-id="e1387-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="e1387-108">Jos muutat säilytystunnistetta tai käytät postilaatikkoon eri säilytyskäytäntöä, voit odottaa, kunnes hallittu kansioavustin käsittelee postilaatikon, tai voit käynnistää hallitun kansion hallinnan suorittamalla Start-ManagedFolderAssistant-cmdlet-otoksen ja käynnistää tietyn postilaatikon.</span><span class="sxs-lookup"><span data-stu-id="e1387-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="e1387-109">Tämän cmdlet-esityksen suorittaminen on hyödyllistä säilytyskäytännön tai säilytystunnisteen asetusten testaamisessa tai vianmäärityksessä.</span><span class="sxs-lookup"><span data-stu-id="e1387-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="e1387-110">Lisätietoja on [ohjeaiheessa Hallitun kansion hallinnan suorittaminen](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="e1387-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="e1387-111">**Ratkaisu:** Käynnistä tietyn postilaatikon hallitun kansion hallintaohjelma suorittamalla seuraava komento:</span><span class="sxs-lookup"><span data-stu-id="e1387-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="e1387-112">Näin voi käydä myös, jos **RetentionHold** on otettu **käyttöön** postilaatikossa.</span><span class="sxs-lookup"><span data-stu-id="e1387-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="e1387-113">Jos postilaatikko on sijoitettu Säilytyspalvelun säilyttämiseen, postilaatikon säilytyskäytäntöä ei käsitellä kyseisenä aikana.</span><span class="sxs-lookup"><span data-stu-id="e1387-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="e1387-114">Lisätietoja RetentionHold-asetuksesta on kohdassa [Postilaatikon säilytyspito](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="e1387-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="e1387-115">**Ratkaisu:**</span><span class="sxs-lookup"><span data-stu-id="e1387-115">**Solution:**</span></span>
    
  - <span data-ttu-id="e1387-116">Tarkista [exo powershellin](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)postilaatikon RetentionHold-asetuksen tila:</span><span class="sxs-lookup"><span data-stu-id="e1387-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="e1387-117">Poista RetentionHold **käytöstä** tietyssä postilaatikossa suorittamalla seuraava komento:</span><span class="sxs-lookup"><span data-stu-id="e1387-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="e1387-118">Suorita nyt hallitun kansion hallintaohjelma uudelleen:</span><span class="sxs-lookup"><span data-stu-id="e1387-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="e1387-119">**Huomautus:** Jos postilaatikon koko on alle 10 megatavua, hallitun kansion hallinta ei käsittele postilaatikkoa automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="e1387-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="e1387-120">Lisätietoja Exchange-hallintakeskuksen säilytyskäytännöistä on seuraavissa ohjeissa:</span><span class="sxs-lookup"><span data-stu-id="e1387-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="e1387-121">Säilytystunnisteet ja säilytyskäytännöt</span><span class="sxs-lookup"><span data-stu-id="e1387-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="e1387-122">Säilytyskäytännön käyttäminen postilaatikoissa</span><span class="sxs-lookup"><span data-stu-id="e1387-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="e1387-123">Säilytystunnisteiden lisääminen tai poistaminen</span><span class="sxs-lookup"><span data-stu-id="e1387-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="e1387-124">Postilaatikkoon sijoitetun pitoon asetetun pidon tyypin tunnistaminen</span><span class="sxs-lookup"><span data-stu-id="e1387-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
