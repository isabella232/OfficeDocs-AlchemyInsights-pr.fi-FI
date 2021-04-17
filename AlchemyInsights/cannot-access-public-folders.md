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
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819509"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook ei voi muodostaa yhteyttä yleisiin kansioihin

Jos yleinen kansion käyttö ei toimi joillakin käyttäjillä, kokeile seuraavaa:

Muodosta yhteys EXO PowerShelliin ja määritä ongelmakäyttäjätilin DefaultPublicFolderMailbox-parametri vastaamaan toimivan käyttäjätilin parametria.

Esimerkki:

Get-Mailbox WorkingUser-| ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Odota vähintään yksi tunti, jotta muutos tulee voimaan.

Jos ongelma ei muutu, noudata [näitä ohjeita](https://aka.ms/pfcte) yleisen kansion käytön ongelmien vianmääritykseen Outlookin avulla.
 
**Voit määrittää, k voivatko käyttäjät käyttää julkisia kansioita Outlookin avulla:**

1.  Käytä Set-CASMailbox <mailboxname> -PublicFolderClientAccess -$true tai $false  
      
    $true: Salli käyttäjien käyttää julkisia kansioita Outlookissa  
      
    $false: Estä käyttäjien pääsy Yleisiin kansioihin Outlookissa. Tämä on oletusarvo.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Huomautus** Tämä toimenpide voi hallita yhteyksiä vain Outlookin työpöytäsovelluksella Windows-asiakassovellohjelmia varten. Käyttäjä voi edelleen käyttää julkisia kansioita OWA:n tai Outlook for Macin avulla.
 
Lisätietoja on kohdassa [Valvotuille yhteyksille Outlookin](https://aka.ms/controlpf)yleisiin kansioihin -tuen ilmoittaminen.