---
title: 932 AADConnectin päivittäminen
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
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9582f1f56e6730e35520b5d79bc245cd74bea0bf4db39b379a7cd133bafc16ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104809"
---
# <a name="upgrade-azure-ad-connect"></a>Azure AD -Näyttöyhteys

Oletusarvoisesti automaattinen päivitys on käytössä Azure AD Näyttöyhteys, mikä varmistaa, että käytössäsi on uusin versio. Voit tarkistaa automaattisen päivityksen asetukset käyttämällä **Get-ADSyncAutoUpgrade-cmdlet-komentoa** Azure AD PowerShellissä. Cmdlet-komento palauttaa jonkin seuraavista arvoista:

- **Käytössä:** Automaattinen päivitys on käytössä.

- **Poissa käytöstä:** Automaattinen päivitys on poistettu käytöstä.

- **Keskeytetty:** Järjestelmä ei ole enää oikeutettu saamaan automaattisia päivityksiä. Tätä arvoa ei voi määrittää; se on järjestelmän asettama.

Lisätietoja on kohdassa [Automaattinen päivitys.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)

Voit ladata Azure AD Näyttöyhteys uusimman version osoitteessa [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
