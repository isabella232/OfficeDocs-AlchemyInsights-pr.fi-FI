---
title: Yleisten kansioiden käyttäminen ei onnistu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: d63a193585cb73c2ce8e160d413db4e837100d33
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341400"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook ei voi muodostaa yhteyttä julkisiin kansioihin

Jos Julkinen-kansion käyttö ei toimi joillekin käyttäjille, kokeile seuraavaa:

Muodosta yhteys EXO PowerShelliin ja Määritä ongelman käyttäjä tilillä oleva Defaunpublic-posti laatikko-parametri vastaamaan toimivan käyttäjä tilin parametria.

Esimerkiksi

Get-Mailbox WorkingUser | FT Defaja Publictillbox, Effectivepublikansiposti laatikko

Posti laatikon ProblemUser-Defauspublicifolder-posti laatikon asettaminen \<value from previous command>

Odota vähintään yksi tunti, ennen kuin muutos tulee voimaan.

Jos ongelma jatkuu, noudata [näitä ohjeita](https://aka.ms/pfcte) , jotta voit suorittaa yleisten kansioiden käyttö ongelmien vian määrityksen Outlookin avulla.
 
Voit **määrittää, ketkä käyttäjät voivat käyttää yleisiä kansioita Outlookin avulla**:

1.  Käytä joukkoa-CASMailbox <mailboxname> -publickansioasiakaskäyttöoikeus $True tai $false  
      
    $true: Salli käyttäjien käyttää yleisiä kansioita Outlookissa  
      
    $false: Estä Outlookin yleisten kansioiden käyttö. Tämä on oletusarvo.  
        
2.  Asetukset-OrganizationConfig-Publiclickshowclient Control $true   
      
**Huomautus** Tämä toiminto sarja voi hallita yhteyksiä vain Windows-asiakas ohjelmien Outlookin Työpöytä versiossa. Käyttäjä voi edelleen käyttää yleisiä kansioita OWA-tai Outlook for Mac-sovelluksessa.
 
Lisä tietoja on kohdassa [valvottavien yhteyksien tuen ilmoittaminen Outlookin julkisissa kansioissa](https://aka.ms/controlpf).