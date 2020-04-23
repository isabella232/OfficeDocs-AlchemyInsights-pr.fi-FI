---
title: Exchange Admin Centerin säilytyskäytännöt eivät toimi
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
ms.openlocfilehash: e2fb22f872be0eefc3b4b78b18cd09baffa66cda
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742430"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="1055b-102">Exchange Admin Centerin säilytyskäytännöt</span><span class="sxs-lookup"><span data-stu-id="1055b-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="1055b-103">**Numero:** Exchange-hallintakeskuksen äskettäin luodut tai päivitetyt säilytyskäytännöt eivät koske postilaatikoita tai kohteita ei siirretä arkistopostilaatikkoon tai poisteta.</span><span class="sxs-lookup"><span data-stu-id="1055b-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="1055b-104">**Perussyitä:**</span><span class="sxs-lookup"><span data-stu-id="1055b-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="1055b-105">Tämä voi johtua siitä, **että hallitun kansion avustaja** ei ole käsitellyt käyttäjän postilaatikkoa.</span><span class="sxs-lookup"><span data-stu-id="1055b-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="1055b-106">Hallitun kansion avustaja yrittää käsitellä kaikki pilvipohjaisen organisaatiosi postilaatikot seitsemän päivän välein.</span><span class="sxs-lookup"><span data-stu-id="1055b-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="1055b-107">Jos muutat säilytystunnistetta tai käytät eri säilytyskäytäntöä postilaatikossa, voit odottaa, kunnes hallitun kansion tuki käsittelee postilaatikon, tai voit käynnistää Hallitun kansion hallinnan suorittamalla Start-ManagedFolderAssistant-cmdlet-tiedoston ja käsitellä tietyn postilaatikon.</span><span class="sxs-lookup"><span data-stu-id="1055b-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="1055b-108">Tämän cmdlet-tiedoston suorittaminen on hyödyllistä säilytyskäytännön tai säilytystunnisteasetusten testaamisessa tai vianmäärityksessä.</span><span class="sxs-lookup"><span data-stu-id="1055b-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="1055b-109">Lisätietoja on [ohjeaiheessa Hallitun kansion hallinnan suorittaminen](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="1055b-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="1055b-110">**Ratkaisu:** Käynnistä tietyn postilaatikon hallitun kansion hallinta:</span><span class="sxs-lookup"><span data-stu-id="1055b-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="1055b-111">Tämä voi tapahtua myös, jos **RetentionHold** on otettu **käyttöön** postilaatikossa.</span><span class="sxs-lookup"><span data-stu-id="1055b-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="1055b-112">Jos postilaatikko on sijoitettu RetentionHold-pitoon, postilaatikon säilytyskäytäntöä ei käsitellä kyseisenä aikana.</span><span class="sxs-lookup"><span data-stu-id="1055b-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="1055b-113">Lisätietoja RetentionHold-asetuksesta on kohdassa [Postilaatikon säilytyspito .](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)</span><span class="sxs-lookup"><span data-stu-id="1055b-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="1055b-114">**Ratkaisu:**</span><span class="sxs-lookup"><span data-stu-id="1055b-114">**Solution:**</span></span>
    
  - <span data-ttu-id="1055b-115">Tarkista tietyn postilaatikon RetentionHold-asetuksen tila [EXO powershell -kohdassa:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="1055b-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="1055b-116">Poista RetentionHold käytöstä tietyssä postilaatikossa **suorittamalla** seuraava komento:</span><span class="sxs-lookup"><span data-stu-id="1055b-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="1055b-117">Suorita hallitun kansion avustaja uudelleen:</span><span class="sxs-lookup"><span data-stu-id="1055b-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="1055b-118">**Huomautus:** Jos postilaatikon koko on pienempi kuin 10 megatavua, hallitun kansion avustaja ei käsittele postilaatikkoa automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="1055b-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="1055b-119">Lisätietoja Exchange-hallintakeskuksen säilytyskäytännöistä on seuraavissa ohjeissa:</span><span class="sxs-lookup"><span data-stu-id="1055b-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="1055b-120">Säilytystunnisteet ja säilytyskäytännöt</span><span class="sxs-lookup"><span data-stu-id="1055b-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="1055b-121">Säilytyskäytännön käyttäminen postilaatikoissa</span><span class="sxs-lookup"><span data-stu-id="1055b-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="1055b-122">Säilytystunnisteiden lisääminen tai poistaminen</span><span class="sxs-lookup"><span data-stu-id="1055b-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="1055b-123">Postilaatikkoon sijoitetun pidon tyypin tunnistaminen</span><span class="sxs-lookup"><span data-stu-id="1055b-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
