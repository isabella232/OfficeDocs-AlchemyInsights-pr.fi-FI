---
title: Salasanojen synkronoinnin vianmääritys
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: c71fce8621057093d23891c26f7b0285fdc8b9ed
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/15/2019
ms.locfileid: "28287141"
---
# <a name="troubleshoot-password-synchronization"></a>Salasanojen synkronoinnin vianmääritys

Jos ei ole salasanoja ovat synkronoituna Azure AD Yhdistä versio 1.1.614.0 tai uudempi ongelmien vianmääritys:
  
1. Avaa uuden Windows PowerShell-istunnon Azure AD yhteyden palvelimeen ja **Suorita järjestelmänvalvojana** -asetusta. 
    
2. Suorita **Set-suorituskäytäntöä RemoteSigned** tai **Set-suorituskäytäntöä rajoittamaton**. 
    
3. Käynnistä ohjattu Azure AD-muodosta.
    
4. Siirry ** lisätehtävät **-sivulla ** vianmääritys **, ja valitse **Seuraava**. 
    
5. Vianmääritys sivulla **vianmäärityksen käynnistäminen Käynnistä** -valikosta PowerShell. 
    
6. Valitse päävalikosta, **Salasanojen synkronoinnin vianmäärityksestä**. 
    
7. Sub-valikosta Valitse **salasana ei toimi ollenkaan**. 
    
 **Tietoja vianmäärityksen tehtävän tulokset**
  
Vianetsinnän tehtävän suorittaa seuraavat tarkistukset:
  
- Tarkistaa, että salasana synkronointitoiminnon Azure AD-vuokralaisen on käytössä.
    
- Vahvistaa Azure AD Yhdistä palvelimeen ei väliaikaisen tilassa.
    
- Jokaisen aiemmin paikalliseen Active Directory Connector (joka vastaa Active Directory-toimialuepuuryhmän):
    
- 
  - Tarkistaa, että salasana synkronointi-ominaisuus on käytössä.
    
  - Etsii salasana syke synkronointitapahtumat Windowsin sovellus-tapahtumalokiin.
    
  - Varten kukin Active Directory-toimialueen paikalliseen Active Directory connector-kohdassa:
    
  - Tarkistaa, että toimialue on käytettävissä Azure AD Yhdistä palvelimeen.
    
  - Vahvistaa, että paikallinen Active Directory connector käyttää Active Directory Domain Services (AD DS)-tilit on oikea käyttäjänimi, salasana ja salasanan synkronointia varten tarvittavat oikeudet.
    
Salasanan synkronointi vianmäärityksen lisäapua Katso [vianmääritys salasanojen synkronoinnin Azure AD Yhdistä synkronoinnissa](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  

