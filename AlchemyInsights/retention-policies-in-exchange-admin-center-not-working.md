---
title: Exchange-hallinta keskuksen säilytys käytännöt eivät toimi
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740507"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="67960-102">Exchange-hallinta keskuksen säilytys käytännöt</span><span class="sxs-lookup"><span data-stu-id="67960-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="67960-103">Jos haluat, että suoritat automaattiset tarkistukset alla mainittuihin asetuksiin, valitse Edellinen-painike <--tämän sivun yläosassa ja kirjoita sitten sen käyttäjän Sähkö posti osoite, jolla on ongelmia säilytys käytäntöjen kanssa.</span><span class="sxs-lookup"><span data-stu-id="67960-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="67960-104">**Ongelma:** Exchange-hallinta keskuksen uudet tai päivitetyt säilytys käytännöt eivät koske posti laatikoita tai kohteita ei siirretä Arkisto posti laatikkoon tai niitä ei poisteta.</span><span class="sxs-lookup"><span data-stu-id="67960-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="67960-105">**Perimmäiset syyt:**</span><span class="sxs-lookup"><span data-stu-id="67960-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="67960-106">Tämä voi johtua siitä, että **Hallittujen kansioiden hallinta** ei ole käsitellyt käyttäjän posti laatikkoa.</span><span class="sxs-lookup"><span data-stu-id="67960-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="67960-107">Hallittujen kansioiden avustaja yrittää käsitellä jokaista pilvipohjaisen organisaatiosi posti laatikkoa kerran seitsemän päivän välein.</span><span class="sxs-lookup"><span data-stu-id="67960-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="67960-108">Jos muutat säilytys tunnisteen tai käytät eri säilytys käytäntöä posti laatikolle, voit odottaa, että hallittujen kansioiden avustaja käsittelee posti laatikkoa, tai voit käynnistää hallitun kansion avustajan käsittelemään tietyn posti laatikon suorittamalla Käynnistä-Managedfoldannestention-cmdlet-toiminnon.</span><span class="sxs-lookup"><span data-stu-id="67960-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="67960-109">Tämän cmdlet-toiminnon suorittaminen on hyödyllistä säilytys käytännön tai säilytyksen tunniste asetusten testaamiseen tai vian määritykseen.</span><span class="sxs-lookup"><span data-stu-id="67960-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="67960-110">Lisä tietoja on Ohje aiheessa [hallitun kansion avustajan suorittaminen](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="67960-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="67960-111">**Ratkaisu:** Käynnistä hallitun kansion avustaja tietylle posti laatikolle suorittamalla seuraava komento:</span><span class="sxs-lookup"><span data-stu-id="67960-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="67960-112">Tämä voi ilmetä myös, jos **RetentionHold** on **otettu käyttöön** posti laatikossa.</span><span class="sxs-lookup"><span data-stu-id="67960-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="67960-113">Jos posti laatikko on asetettu RetentionHold-kohtaan, posti laatikon säilytys käytäntöä ei prosessoida tuona aikana.</span><span class="sxs-lookup"><span data-stu-id="67960-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="67960-114">Lisä tietoja on kohdassa RetentionHold-asetus Katso: [Posti laatikon säilytyksen pito](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="67960-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="67960-115">**Ratkaisu**</span><span class="sxs-lookup"><span data-stu-id="67960-115">**Solution:**</span></span>
    
  - <span data-ttu-id="67960-116">Tarkasta RetentionHold-asetuksen tila tietyssä posti laatikossa [EXO PowerShellin](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)avulla:</span><span class="sxs-lookup"><span data-stu-id="67960-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="67960-117">Suorita seuraava komento, jos haluat poistaa RetentionHold-toiminnon **käytöstä** tietyssä posti laatikossa:</span><span class="sxs-lookup"><span data-stu-id="67960-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="67960-118">Suorita sitten hallitun kansion avustaja uudelleen:</span><span class="sxs-lookup"><span data-stu-id="67960-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="67960-119">**Huomautus:** Jos posti laatikko on pienempi kuin 10 Mt, hallittujen kansioiden hallinta ohjelma ei käsittele posti laatikkoa automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="67960-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="67960-120">Lisä tietoja Exchange-hallinta keskuksen säilytys käytännöistä on kohdassa:</span><span class="sxs-lookup"><span data-stu-id="67960-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="67960-121">Säilytys Tunnisteet ja säilytys käytännöt</span><span class="sxs-lookup"><span data-stu-id="67960-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="67960-122">Säilytys käytännön käyttäminen posti laatikoissa</span><span class="sxs-lookup"><span data-stu-id="67960-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="67960-123">Säilytys tunnisteiden lisääminen tai poistaminen</span><span class="sxs-lookup"><span data-stu-id="67960-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="67960-124">Posti laatikkoon sijoitetun pidon tyypin selvittäminen</span><span class="sxs-lookup"><span data-stu-id="67960-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
