---
title: Säilytyskäytännöt Keskikaiuttimen Admin ei toimi
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 9f4a175239bc20aaf489615da63ef35002030a70
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/28/2019
ms.locfileid: "35369662"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="0d59f-102">Säilytyskäytännöt-Exchange-hallintakeskukseen</span><span class="sxs-lookup"><span data-stu-id="0d59f-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="0d59f-103">**Ongelma:** Äskettäin luotu tai päivitetty Exchange Admin Centerissä säilytyskäytännöt soveltavat ei postilaatikoihin tai kohteita ei Arkistoi postilaatikko siirretään tai poistetaan.</span><span class="sxs-lookup"><span data-stu-id="0d59f-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="0d59f-104">**Pääsyyt:**</span><span class="sxs-lookup"><span data-stu-id="0d59f-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="0d59f-105">Tämä voi johtua siitä että **Hallitun kansion avustajan** ei käsitelty käyttäjän postilaatikkoon.</span><span class="sxs-lookup"><span data-stu-id="0d59f-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="0d59f-106">Hallitun kansion avustajan yrittää käsitellä jokaisen postilaatikon pilvipohjainen organisaatiosi seitsemän päivän välein.</span><span class="sxs-lookup"><span data-stu-id="0d59f-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="0d59f-107">Jos muutat pidätys tunnisteen tai soveltaa eri säilytyskäytäntö postilaatikkoon, voit odottaa, kunnes hallitun kansion avustaa käsittelee postilaatikon, tai voit suorittaa Start-ManagedFolderAssistant-cmdlet-komento Käynnistä-hallitun kansion avustajan käsittelemään tiettyä postilaatikko.</span><span class="sxs-lookup"><span data-stu-id="0d59f-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="0d59f-108">Käytössä tämä cmdlet-komento on hyödyllinen testaamisessa ja vianmäärityksessä tai säilytyskäytäntö säilytysasetukset tunniste.</span><span class="sxs-lookup"><span data-stu-id="0d59f-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="0d59f-109">Saat lisätietoja seuraavasta [suorittaa hallitun kansion avustajan](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="0d59f-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="0d59f-110">**Ratkaisu:** Suorita seuraava komento käynnistää-hallitun kansion avustajan tietylle postilaatikolle:</span><span class="sxs-lookup"><span data-stu-id="0d59f-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="0d59f-111">Tämä saattaa myös ilmetä, jos **RetentionHold** on **otettu** käyttöön postilaatikon.</span><span class="sxs-lookup"><span data-stu-id="0d59f-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="0d59f-112">Jos RetentionHold sijoitettu postilaatikko, säilytyskäytäntö-postilaatikko ei käsitellä samaan aikaan.</span><span class="sxs-lookup"><span data-stu-id="0d59f-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="0d59f-113">Saat enemmän informaton-RetentionHold asetus Katso: [Postilaatikon pidätys pidä](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="0d59f-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="0d59f-114">**Ratkaisu:**</span><span class="sxs-lookup"><span data-stu-id="0d59f-114">**Solution:**</span></span>
    
  - <span data-ttu-id="0d59f-115">Tietyn postilaatikon [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)-RetentionHold-asetuksen tarkistaminen:</span><span class="sxs-lookup"><span data-stu-id="0d59f-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="0d59f-116">Suorita seuraava komento **poistaa** RetentionHold tietyn postilaatikon:</span><span class="sxs-lookup"><span data-stu-id="0d59f-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="0d59f-117">Nyt uudelleen suorittaa hallitun kansion avustajan:</span><span class="sxs-lookup"><span data-stu-id="0d59f-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="0d59f-118">**Huomautus:** Jos postilaatikko on alle 10 Mt, hallitun kansion avustajan ei automaattisesti käsittelee postilaatikon.</span><span class="sxs-lookup"><span data-stu-id="0d59f-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
  