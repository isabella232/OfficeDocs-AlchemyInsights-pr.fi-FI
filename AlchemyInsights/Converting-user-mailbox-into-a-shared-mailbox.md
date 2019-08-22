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
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496396"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a><span data-ttu-id="d46f3-102">Muuntaa käyttäjän postilaatikko jaetusta postilaatikosta</span><span class="sxs-lookup"><span data-stu-id="d46f3-102">Convert a user mail box into a shared mailbox</span></span>

<span data-ttu-id="d46f3-103">Voit muuntaa käyttäjän postilaatikon jaetun Exchange-postilaatikon vain jos käyttäjällä on Exchange-käyttöoikeus.</span><span class="sxs-lookup"><span data-stu-id="d46f3-103">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="d46f3-104">Kun postilaatikko on muunnettu, sitä edelleen, koska tämä luettelo sisältää jaettujen postilaatikoiden näy aktiivisten käyttäjien luettelossa.</span><span class="sxs-lookup"><span data-stu-id="d46f3-104">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="d46f3-105">Kuitenkin muunnettu postilaatikon tulee myös näkyviin jaettu postilaatikko-luettelosta.</span><span class="sxs-lookup"><span data-stu-id="d46f3-105">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="d46f3-106">Jos yrität muuttaa postilaatikon Exchangen hallintakonsolissa ja muuntaminen epäonnistuu, tyhjennä selaimen välimuisti ja evästeet ja yritä uudelleen.</span><span class="sxs-lookup"><span data-stu-id="d46f3-106">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="d46f3-107">Jos näppäimistö ei edelleenkään toimi, yritä muuntaa postilaatikko Exchange Management Shell-suorittamalla seuraava komento:</span><span class="sxs-lookup"><span data-stu-id="d46f3-107">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="d46f3-108">Postilaatikon muuntaminen tietoja on käytettävissä enemmän, [muuntaa jaetun postilaatikon käyttäjän postilaatikkoon](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span><span class="sxs-lookup"><span data-stu-id="d46f3-108">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span></span>
  
