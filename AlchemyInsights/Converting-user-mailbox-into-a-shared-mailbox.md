---
title: Jaetun postilaatikon käyttäjän postilaatikon muuntaminen?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 4da54121763fd33aa111f3bb3c26963cd271dc51
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906729"
---
<span data-ttu-id="e3536-p101">Voit muuntaa käyttäjän postilaatikon jaetun Exchange-postilaatikon vain jos käyttäjällä on Exchange-käyttöoikeus. Kun postilaatikko on muunnettu, sitä edelleen, koska tämä luettelo sisältää jaettujen postilaatikoiden näy aktiivisten käyttäjien luettelossa. Kuitenkin muunnettu postilaatikon tulee myös näkyviin jaettu postilaatikko-luettelosta.</span><span class="sxs-lookup"><span data-stu-id="e3536-p101">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license. After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes. However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="e3536-p102">Jos yrität muuttaa postilaatikon Exchangen hallintakonsolissa ja muuntaminen epäonnistuu, tyhjennä selaimen välimuisti ja evästeet ja yritä uudelleen. Jos näppäimistö ei edelleenkään toimi, yritä muuntaa postilaatikko Exchange Management Shell-suorittamalla seuraava komento:</span><span class="sxs-lookup"><span data-stu-id="e3536-p102">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again. If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="e3536-107">Postilaatikon muuntaminen tietoja on käytettävissä enemmän, [muuntaa jaetun postilaatikon käyttäjän postilaatikkoon](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span><span class="sxs-lookup"><span data-stu-id="e3536-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
