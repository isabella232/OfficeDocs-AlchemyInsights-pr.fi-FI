---
title: Säilytyskäytännöt Keskikaiuttimen Admin ei toimi
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: c9061fa728edaab6575a7b1027783e56739a6d14
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/12/2019
ms.locfileid: "29934989"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="1172d-102">Säilytyskäytännöt-Exchange-hallintakeskukseen</span><span class="sxs-lookup"><span data-stu-id="1172d-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="1172d-103">**Ongelma:** Äskettäin luotu tai päivitetty Exchange Admin Centerissä säilytyskäytännöt soveltavat ei postilaatikoihin tai kohteita ei Arkistoi postilaatikko siirretään tai poistetaan.</span><span class="sxs-lookup"><span data-stu-id="1172d-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="1172d-104">**Pääsyyt:**</span><span class="sxs-lookup"><span data-stu-id="1172d-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="1172d-p101">Tämä voi johtua siitä että **Hallitun kansion avustajan** ei käsitelty käyttäjän postilaatikkoon. Hallitun kansion avustajan yrittää käsitellä jokaisen postilaatikon pilvipohjainen organisaatiosi seitsemän päivän välein. Jos muutat pidätys tunnisteen tai soveltaa eri säilytyskäytäntö postilaatikkoon, voit odottaa, kunnes hallitun kansion avustaa käsittelee postilaatikon, tai voit suorittaa Start-ManagedFolderAssistant-cmdlet-komento Käynnistä-hallitun kansion avustajan käsittelemään tiettyä postilaatikko. Käytössä tämä cmdlet-komento on hyödyllinen testaamisessa ja vianmäärityksessä tai säilytyskäytäntö säilytysasetukset tunniste. Saat lisätietoja seuraavasta [suorittaa hallitun kansion avustajan](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="1172d-p101">This may be because the **Managed Folder Assistant** has not processed the user's mailbox. The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days. If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox. Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings. For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="1172d-110">**Ratkaisu:** Suorita seuraava komento käynnistää-hallitun kansion avustajan tietylle postilaatikolle:</span><span class="sxs-lookup"><span data-stu-id="1172d-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="1172d-p102">Tämä saattaa myös ilmetä, jos **RetentionHold** on **otettu** käyttöön postilaatikon. Jos RetentionHold sijoitettu postilaatikko, säilytyskäytäntö-postilaatikko ei käsitellä samaan aikaan. Saat enemmän informaton-RetentionHold asetus Katso: [Postilaatikon pidätys pidä](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="1172d-p102">This may also be occur if **RetentionHold** has been **enabled** on the mailbox. If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time. For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="1172d-114">**Ratkaisu:**</span><span class="sxs-lookup"><span data-stu-id="1172d-114">**Solution:**</span></span>
    
  - <span data-ttu-id="1172d-115">Tietyn postilaatikon [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)-RetentionHold-asetuksen tarkistaminen:</span><span class="sxs-lookup"><span data-stu-id="1172d-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="1172d-116">Suorita seuraava komento **poistaa** RetentionHold tietyn postilaatikon:</span><span class="sxs-lookup"><span data-stu-id="1172d-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="1172d-117">Nyt uudelleen suorittaa hallitun kansion avustajan:</span><span class="sxs-lookup"><span data-stu-id="1172d-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="1172d-118">**Huomautus:** Jos postilaatikko on alle 10 Mt, hallitun kansion avustajan ei automaattisesti käsittelee postilaatikon.</span><span class="sxs-lookup"><span data-stu-id="1172d-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

