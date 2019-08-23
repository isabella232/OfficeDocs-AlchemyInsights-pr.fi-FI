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
ms.openlocfilehash: 5d7b62546397c13b37540e8797b31123b2880280
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551340"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="800be-102">Säilytyskäytännöt-Exchange-hallintakeskukseen</span><span class="sxs-lookup"><span data-stu-id="800be-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="800be-103">**Ongelma:** Äskettäin luotu tai päivitetty Exchange Admin Centerissä säilytyskäytännöt soveltavat ei postilaatikoihin tai kohteita ei Arkistoi postilaatikko siirretään tai poistetaan.</span><span class="sxs-lookup"><span data-stu-id="800be-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="800be-104">**Pääsyyt:**</span><span class="sxs-lookup"><span data-stu-id="800be-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="800be-105">Tämä voi johtua siitä että **Hallitun kansion avustajan** ei käsitelty käyttäjän postilaatikkoon.</span><span class="sxs-lookup"><span data-stu-id="800be-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="800be-106">Hallitun kansion avustajan yrittää käsitellä jokaisen postilaatikon pilvipohjainen organisaatiosi seitsemän päivän välein.</span><span class="sxs-lookup"><span data-stu-id="800be-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="800be-107">Jos muutat pidätys tunnisteen tai soveltaa eri säilytyskäytäntö postilaatikkoon, voit odottaa, kunnes hallitun kansion avustaa käsittelee postilaatikon, tai voit suorittaa Start-ManagedFolderAssistant-cmdlet-komento Käynnistä-hallitun kansion avustajan käsittelemään tiettyä postilaatikko.</span><span class="sxs-lookup"><span data-stu-id="800be-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="800be-108">Käytössä tämä cmdlet-komento on hyödyllinen testaamisessa ja vianmäärityksessä tai säilytyskäytäntö säilytysasetukset tunniste.</span><span class="sxs-lookup"><span data-stu-id="800be-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="800be-109">Saat lisätietoja seuraavasta [suorittaa hallitun kansion avustajan](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="800be-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="800be-110">**Ratkaisu:** Suorita seuraava komento käynnistää-hallitun kansion avustajan tietylle postilaatikolle:</span><span class="sxs-lookup"><span data-stu-id="800be-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="800be-111">Tämä saattaa myös ilmetä, jos **RetentionHold** on **otettu** käyttöön postilaatikon.</span><span class="sxs-lookup"><span data-stu-id="800be-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="800be-112">Jos RetentionHold sijoitettu postilaatikko, säilytyskäytäntö-postilaatikko ei käsitellä samaan aikaan.</span><span class="sxs-lookup"><span data-stu-id="800be-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="800be-113">Saat enemmän informaton-RetentionHold asetus Katso: [Postilaatikon pidätys pidä](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="800be-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="800be-114">**Ratkaisu:**</span><span class="sxs-lookup"><span data-stu-id="800be-114">**Solution:**</span></span>
    
  - <span data-ttu-id="800be-115">Tietyn postilaatikon [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)-RetentionHold-asetuksen tarkistaminen:</span><span class="sxs-lookup"><span data-stu-id="800be-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="800be-116">Suorita seuraava komento **poistaa** RetentionHold tietyn postilaatikon:</span><span class="sxs-lookup"><span data-stu-id="800be-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="800be-117">Nyt uudelleen suorittaa hallitun kansion avustajan:</span><span class="sxs-lookup"><span data-stu-id="800be-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="800be-118">**Huomautus:** Jos postilaatikko on alle 10 Mt, hallitun kansion avustajan ei automaattisesti käsittelee postilaatikon.</span><span class="sxs-lookup"><span data-stu-id="800be-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="800be-119">Saat lisätietoja Exchange-Admin Centerissä säilytyskäytännöt:</span><span class="sxs-lookup"><span data-stu-id="800be-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="800be-120">Pidätys tunnisteet ja säilytyskäytäntöjä</span><span class="sxs-lookup"><span data-stu-id="800be-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="800be-121">Käytä säilytyskäytäntöä postilaatikot</span><span class="sxs-lookup"><span data-stu-id="800be-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="800be-122">Lisää tai poistaa tunnisteet pidätys</span><span class="sxs-lookup"><span data-stu-id="800be-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="800be-123">Miten tunnistaa pidon tyyppi sijoitettu postilaatikkoon</span><span class="sxs-lookup"><span data-stu-id="800be-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
