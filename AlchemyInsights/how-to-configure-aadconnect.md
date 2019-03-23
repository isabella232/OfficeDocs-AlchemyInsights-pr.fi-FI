---
title: 646 AADConnect määrittämisestä
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6cc4afb4b0f67fb76ecc7ff8f564b1cd36cc291c
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/22/2019
ms.locfileid: "30779509"
---
# <a name="configure-sync-features"></a>Synkronoinnin ominaisuuksien määrittäminen

Azure AD Connect on useita ominaisuuksia, jotka ovat oletusarvoisesti käytössä tai jotka voidaan ottaa käyttöön myöhemmin. Jotkin ominaisuudet edellyttävät lisämäärityksiä ympäristöissä.
  
- Azure AD [suodatus](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) rajoitusten objektit synkronoidaan. Tietokonetilit synkronoidaan oletusarvon, kaikki käyttäjät, yhteyshenkilöt, ryhmät ja Windows 10 mukaan. Voit sisällyttää tai jättää pois toimialueisiin, organisaatioyksiköihin tai muita määritteitä perustuvat objektit. 
    
- [Salasana hash synkronointi:](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) Synkronoi Azure AD paikalliseen Active Directory-salasanan hajautuksen. Tämä mahdollistaa salasanojen hallinta yhdessä paikassa, mutta käyttää samaa salasanaa molemmissa tiloissa ja solmuryhmän ympäristöissä. Active Directory on virallinen lähde, koska voit käyttää omia salasanakäytännöt. 
    
- [Omatoiminen salasanan (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) käyttäjät voivat palauttaa omat salasanansa solmuryhmässä otettaessa yhteyttä paikalliseen Salasanakäytäntö edelleen. 
    
- [Takaisinkirjoitus laitteen](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) avulla rekisteröity laitteet voidaan kirjoittaa takaisin paikalliseen Active Directoryyn, joten niitä voidaan käyttää ehdollisen käyttöoikeuden Azure AD. 
    
- [Estä vahingossa poistaa](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) on oletusarvoisesti estämään liian monta samanaikaista objektin poistot (yli 500 objektien synkronointi kohti). Voit muuttaa tätä asetusta vastaamaan organisaation tarpeita. 
    
- [Automaattinen päivitys](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) on käytössä oletusarvoisesti express asennukset ja varmistamaan Azure AD Yhdistä versio on aina ajan tasalla. 
    

