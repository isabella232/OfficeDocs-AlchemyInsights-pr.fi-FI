---
title: Salasanan synkronointiin liittyviä ongelmia
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732507"
---
# <a name="troubleshoot-password-synchronization"></a>Salasanan synkronointiin liittyviä ongelmia

Sellaisten ongelmien vianmääritys, joissa salasanoja ei synkronoida Azure AD Connectin version 1.1.614.0 tai uudemman kanssa:
  
1. Avaa uusi Windows PowerShell -istunto Azure AD Connect -palvelimessa **Suorita järjestelmänvalvojana** -asetuksen avulla.

2. Suorita **Set-ExecutionPolicy RemoteSigned** tai **Set-ExecutionPolicy rajoittamaton**.

3. Käynnistä ohjattu Azure AD Connect -toiminto.

4. Siirry **Lisätehtävät-sivulle,** valitse **Vianmääritys**ja valitse **Seuraava**.

5. Käynnistä Vianmääritys-valikon **vianmääritysvalikko PowerShellissä** valitsemalla Vianmääritys-sivulla Käynnistä.

6. Valitse päävalikosta **Salasanan synkronoinnin vianmääritys**.

7. Valitse alivalikosta **Salasanan synkronointi ei toimi lainkaan**.

**Tietoja vianmääritystehtävän tuloksista**
  
Vianmääritystehtävä suorittaa seuraavat tarkistukset:
  
- Tarkistaa, että salasanan synkronointiominaisuus on käytössä Azure AD -vuokraajassa.

- Tarkistaa, että Azure AD Connect -palvelin ei ole valmistelutilassa.

- Kunkin paikallisen Active Directory -yhdistimen osalta (joka vastaa olemassa olevaa Active Directory -toimialuepuuryhmään):

- 
  - Tarkistaa, että salasanan synkronointiominaisuus on käytössä.

  - Etsii salasanan synkronoinnin syketapahtumia Windowsin sovellustapahtumalokeista.

  - Kunkin paikallisen Active Directory -yhdistimen alla olevan Active Directory -toimialueen osalta:

  - Tarkistaa, että toimialue on tavoitettavissa Azure AD Connect -palvelimesta.

  - Tarkistaa, että paikallisen Active Directory -yhdistimen käyttämien Active Directory -toimialueen palveluiden (AD DS) tileillä on oikea käyttäjätunnus, salasana ja salasanasynkronointiin tarvittavat käyttöoikeudet.

Lisätietoja salasanan synkronoinnin vianmäärityksestä on [ohjeaiheessa Salasanan synkronoinnin vianmääritys Azure AD Connect -synkronoinnin kanssa](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  