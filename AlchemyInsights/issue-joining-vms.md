---
title: Ongelma liittyminen VMS:iin
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885212"
---
# <a name="issue-joining-vms"></a>Ongelma liittyminen VMS:iin

Voit ratkaista ongelmia, jotka ilmenevät, kun yrität liittyä VMS-isiin, toimimalla seuraavasti:

1. Yritä kirjautua sisään **UPN-muodossa** (esimerkiksi "joeuser@contoso.com") **SAMAccountName-muodon** (CONTOSO\joeuser) sijaan.
2. Varmista, että olet ottanut salasanasynkronoinnin käyttöön aloitusoppaan *ohjeiden* mukaisesti.
3. Varmista, että kyseinen käyttäjätili ei ole ulkoinen tili Azure AD -vuokraajassa. Ulkoiset käyttäjät eivät voi kirjautua hallittuun toimialueeseen, koska Azure AD -toimialuepalveluilla ei ole tällaisten käyttäjätilien tunnistetietoja.
4. Jos kyseinen käyttäjätili on vain pilvipalvelun käyttäjätili, varmista, että käyttäjät ovat vaihtaneet salasanansa Azure AD -toimialueen palveluiden käytön jälkeen. Tämä vaihe aiheuttaa Azure AD -toimialuepalvelujen edellyttämät tunnistetietojen hasheet.
5. Jos ongelmaan liittyvät käyttäjätilit synkronoidaan paikallisesta hakemistosta, varmista, että Azure AD Connectin suositeltu julkaisu on määritetty suorittamaan täysi synkronointi.
6. Jos ongelmat jatkuvat vaiheen 4 vahvistuksen jälkeen, suorita seuraavat komennot synkronointikoneesta:
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.