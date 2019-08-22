---
title: 646 AADConnect määrittämisestä
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 316d7253494c55a9bc94797d493897c2ddec516c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36541582"
---
# <a name="configure-sync-features"></a>Synkronoinnin ominaisuuksien määrittäminen

Azure AD Connect on useita ominaisuuksia, jotka ovat oletusarvoisesti käytössä tai jotka voidaan ottaa käyttöön myöhemmin. Jotkin ominaisuudet edellyttävät lisämäärityksiä ympäristöissä.

- Azure AD [suodatus](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) rajoitusten objektit synkronoidaan. Tietokonetilit synkronoidaan oletusarvon, kaikki käyttäjät, yhteyshenkilöt, ryhmät ja Windows 10 mukaan. Voit sisällyttää tai jättää pois toimialueisiin, organisaatioyksiköihin tai muita määritteitä perustuvat objektit.

- [Salasana hash synkronoinnin](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) Synkronoi Azure AD paikalliseen Active Directory-salasanan hajautuksen. Tämä mahdollistaa salasanojen hallinta yhdessä paikassa, mutta käyttää samaa salasanaa molemmissa tiloissa ja solmuryhmän ympäristöissä. Active Directory on virallinen lähde, koska voit käyttää omia salasanakäytännöt.

- [Omatoiminen salasanan (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) käyttäjät voivat palauttaa omat salasanansa solmuryhmässä otettaessa yhteyttä paikalliseen Salasanakäytäntö edelleen.

- [Takaisinkirjoitus laitteen](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) avulla rekisteröity laitteet voidaan kirjoittaa takaisin paikalliseen Active Directoryyn, joten niitä voidaan käyttää ehdollisen käyttöoikeuden Azure AD.

- [Estä vahingossa poistaa](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) on oletusarvoisesti estämään liian monta samanaikaista objektin poistot (yli 500 objektien synkronointi kohti). Voit muuttaa tätä asetusta vastaamaan organisaation tarpeita.

- [Automaattinen päivitys](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) on käytössä oletusarvoisesti express asennukset ja varmistamaan Azure AD Yhdistä versio on aina ajan tasalla.
