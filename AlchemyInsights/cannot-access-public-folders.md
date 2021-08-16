---
title: Julkisten kansioiden käyttö ei ole käytettävissä
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996627"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook ei voi muodostaa yhteyttä yleisiin kansioihin

Jos yleinen kansion käyttö ei toimi joillakin käyttäjillä, kokeile seuraavaa:

Näyttöyhteys EXO PowerShelliin ja määritä ongelmakäyttäjätilin DefaultPublicFolderMailbox-parametri vastaamaan toimivan käyttäjätilin parametria.

Esimerkki:

Get-Mailbox WorkingUser-| ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Odota vähintään yksi tunti, jotta muutos tulee voimaan.

Jos ongelma ei muutu, noudata [näitä ohjeita](https://aka.ms/pfcte) yleisen kansion käytön ongelmien vianmääritykseen Outlook.
 
**Voit määrittää, k voivatko käyttäjät käyttää julkisia kansioita Outlook:**

1.  Käytä Set-CASMailbox <mailboxname> -PublicFolderClientAccess -$true tai $false  
      
    $true: Salli käyttäjien käyttää Outlook  
      
    $false: Voit estää Outlook:n julkisten kansioiden Outlook. Tämä on oletusarvo.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Huomautus** Tämä toimenpide voi hallita yhteyksiä vain Outlook työpöytäsovelluksessa Windows kanssa. Käyttäjä voi edelleen käyttää julkisia kansioita OWA:n tai Outlook for Mac.
 
Lisätietoja on kohdassa [Valvotuille yhteyksille yleisille](https://aka.ms/controlpf)kansioille ilmoittava tuki Outlook.