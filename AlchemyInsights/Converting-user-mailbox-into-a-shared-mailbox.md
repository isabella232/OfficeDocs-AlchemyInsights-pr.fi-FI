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
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a>Muuntaa käyttäjän postilaatikko jaetusta postilaatikosta

Voit muuntaa käyttäjän postilaatikon jaetun Exchange-postilaatikon vain jos käyttäjällä on Exchange-käyttöoikeus. Kun postilaatikko on muunnettu, sitä edelleen, koska tämä luettelo sisältää jaettujen postilaatikoiden näy aktiivisten käyttäjien luettelossa. Kuitenkin muunnettu postilaatikon tulee myös näkyviin jaettu postilaatikko-luettelosta. 
  
Jos yrität muuttaa postilaatikon Exchangen hallintakonsolissa ja muuntaminen epäonnistuu, tyhjennä selaimen välimuisti ja evästeet ja yritä uudelleen. Jos näppäimistö ei edelleenkään toimi, yritä muuntaa postilaatikko Exchange Management Shell-suorittamalla seuraava komento:
  
```
Set-Mailbox -Type Shared
```

Postilaatikon muuntaminen tietoja on käytettävissä enemmän, [muuntaa jaetun postilaatikon käyttäjän postilaatikkoon](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).
  
