---
title: 646 AADConnectin määrittäminen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722533"
---
# <a name="configure-sync-features"></a>Synkronointiominaisuuksien määrittäminen

Azure AD Connect sisältää useita ominaisuuksia, jotka ovat oletusarvoisesti käytössä tai jotka voidaan ottaa käyttöön myöhemmin. Jotkin ominaisuudet edellyttävät lisämäärityksiä tietyissä ympäristöissä.

- [Suodatus](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) rajoittaa objektien synkronoinnin Azure AD:hen. Oletusarvon mukaan kaikki käyttäjät, yhteystiedot, ryhmät ja Windows 10 -tietokonetilit synkronoidaan. Voit sisällyttää tai jättää pois objekteja, jotka perustuvat toimialueisiin, oUs-kohteisiin tai muihin määritteisiin.

- [Salasanan hajautussynkronointi](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synkronoi salasanan hajautusarvonsa paikallisesta Active Directorysta Azure AD:hen. Tämä mahdollistaa salasanojen hallinnan yhdessä sijainnissa, mutta saman salasanan käyttäminen sekä paikallisissa että pilviympäristöissä. Koska Active Directory on hallitseva lähde, voit käyttää omia salasanakäytäntöjäsi.

- [Itsepalvelusalasanan nollauksen (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) avulla käyttäjät voivat nollata omat salasanansa pilvessä ja silti soveltaa paikallista salasanakäytäntöä.

- [Laitteen takaisinkirjoitus](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) mahdollistaa azure AD:n rekisteröityjen laitteiden kirjoittamisen takaisin paikalliseen Active Directoryyn, jotta niitä voidaan käyttää ehdolliseen käyttöön.

- [Estä vahingossa tapahtuvat poistot](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) on oletusarvoisesti käytössä, jotta vältettäisiin liian monta samanaikaista objektien poistoa (yli 500 objektia synkronointia kohden). Voit muuttaa tätä asetusta organisaatiosi tarpeiden mukaan.

- [Automaattinen päivitys](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) on oletusarvoisesti käytössä pika-asennuksissa, ja se auttaa varmistamaan, että Azure AD Connectin versio on aina ajan tasalla.
