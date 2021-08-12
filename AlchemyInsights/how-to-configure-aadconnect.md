---
title: 646 AADConnectin määrittäminen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963640"
---
# <a name="configure-sync-features"></a>Synkronointiominaisuuksien määrittäminen

Azure AD Näyttöyhteys sisältää useita ominaisuuksia, jotka ovat oletusarvoisesti käytössä tai jotka voit ottaa myöhemmin käyttöön. Jotkin ominaisuudet edellyttävät lisämäärityksiä tietyissä ympäristöissä.

- [Suodatusrajat,](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) jotka objektit synkronoidaan Azure AD:lle. Oletusarvoisesti kaikki käyttäjät, yhteystiedot, ryhmät Windows 10 tietokonetilit synkronoidaan. Voit sisällyttää tai jättää pois toimialueisiin, OUs-ominaisuuksiin tai muihin määritteeseen perustuvia objekteja.

- [Salasanojen salasanojen](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) hash-synkronointi synkronoi paikallisen Active Directoryn ja Azure AD:n salasanojen hash-tiedot. Näin salasanojen hallinta on mahdollista yhdessä paikassa, mutta samaa salasanaa voidaan käyttää sekä paikallisissa ympäristöissä että pilviympäristöissä. Koska Active Directory on olennainen lähde, voit käyttää omia salasanakäytäntöjäsi.

- [Omatoiminen salasanan vaihto (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) mahdollistaa omien salasanojen vaihtamisen pilvipalvelussa samalla, kun he ovat edelleen paikallisen salasanakäytännön käytössä.

- [Laitteen takaisinkirjoittamisen](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) avulla azure AD:ssä rekisteröidyt laitteet voidaan kirjoittaa takaisin paikalliseen Active Directoryyn, jotta niitä voidaan käyttää ehdolliseen käyttöön.

- [Estä tahattoman poistamisen estäminen](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) on oletusarvoisesti käytössä, jotta voit estää liian monta samanaikaista objektien poistoa (yli 500 objektia synkronoinnissa). Voit muuttaa tätä asetusta organisaatiosi tarpeiden mukaan.

- [Automaattinen päivitys](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) on oletusarvoisesti käytössä pika-asennuksissa ja auttaa varmistamaan, että Azure AD Näyttöyhteys on aina ajan tasalla.
