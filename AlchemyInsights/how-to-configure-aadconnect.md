---
title: 646 AADConnect-asetusten määrittäminen
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
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704486"
---
# <a name="configure-sync-features"></a>Synkronointi ominaisuuksien määrittäminen

Azure AD Connect sisältää useita ominaisuuksia, jotka ovat oletusarvoisesti käytössä tai jotka voit ottaa käyttöön myöhemmin. Jotkin ominaisuudet vaativat lisä määrityksiä tietyissä ympäristöissä.

- [Suodattaminen](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) rajoittaa objektien synkronoinnin Azure AD:hen. Oletusarvoisesti kaikki käyttäjät, yhteys tiedot, ryhmät ja Windows 10-tieto kone tunnukset synkronoidaan. Voit sisällyttää tai jättää pois objekteja toimi alueiden, organisaatio yksiköiden tai muiden määritteiden perusteella.

- [Salasana hajautus synkronointi](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) Synkronoi Sala sanan hajautus arvon paikallisesta Active Directorysta Azure AD:hen. Tämä mahdollistaa Sala sanojen hallinnan yhdessä sijainnissa, mutta käyttää samaa Sala sanaa sekä paikallisessa että pilvi ympäristössä. Koska Active Directory on määräävä lähde, voit käyttää omaa salasana käytäntöä.

- [Omatoiminen Sala sanan palautus (sspr)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) mahdollistaa sen, että käyttäjät voivat vaihtaa Sala sanansa pilvi palvelussa, mutta silti ottaa käyttöön paikallisen salasana käytäntönsä.

- [Laitteen takaisinkirjoitus](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) mahdollistaa sen, että Azure AD:ssä rekisteröityneet laitteet voidaan kirjoittaa takaisin paikalliseen Active Directoryyn, jotta niitä voidaan käyttää ehdollisen käytön aikana.

- [Estä tahattomat poistot](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) ovat oletusarvoisesti käytössä, jotta estetään liian monta samanaikaista objektien poistoa (yli 500 objektia synkronoinnin aikana). Voit muuttaa tätä asetusta vastaamaan organisaatiosi tarpeita.

- [Automaattinen päivitys](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) on oletusarvoisesti käytössä pikaasennuksissa ja auttaa varmistamaan, että Azure AD Connect-versiosi on aina ajan tasalla.
