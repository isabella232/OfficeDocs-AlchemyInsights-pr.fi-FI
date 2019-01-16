---
title: Jaetun postilaatikon käyttäjän postilaatikon muuntaminen?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Priority
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 22ad1b3fb818b40bcd77974031735f931e986968
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/15/2019
ms.locfileid: "28287375"
---
Voit muuntaa käyttäjän postilaatikon jaetun Exchange-postilaatikon vain jos käyttäjällä on Exchange-käyttöoikeus. Kun postilaatikko on muunnettu, sitä edelleen, koska tämä luettelo sisältää jaettujen postilaatikoiden näy aktiivisten käyttäjien luettelossa. Kuitenkin muunnettu postilaatikon tulee myös näkyviin jaettu postilaatikko-luettelosta. 
  
Jos yrität muuttaa postilaatikon Exchangen hallintakonsolissa ja muuntaminen epäonnistuu, tyhjennä selaimen välimuisti ja evästeet ja yritä uudelleen. Jos näppäimistö ei edelleenkään toimi, yritä muuntaa postilaatikko Exchange Management Shell-suorittamalla seuraava komento:
  
```
Set-Mailbox -Type Shared
```

Postilaatikon muuntaminen tietoja on käytettävissä enemmän, [muuntaa jaetun postilaatikon käyttäjän postilaatikkoon](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).
  
