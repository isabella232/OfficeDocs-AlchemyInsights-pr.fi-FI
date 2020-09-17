---
title: 932 päivitys AADConnect
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
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806036"
---
# <a name="upgrade-azure-ad-connect"></a>Azure AD Connect-päivitys

Oletusarvoisesti automaattinen päivitys on käytössä Azure AD Connectin avulla, mikä auttaa varmistamaan, että käytössäsi on uusin versio. Voit tarkistaa automaattiset päivitys asetukset käyttämällä **Get-ADSyncAutoUpgrade-cmdlet-** komennolla Azure AD PowerShellissä. Cmdlet-komento palauttaa jonkin seuraavista arvoista:

- **Käytössä**: Automaattinen päivitys on käytössä.

- Ei **käytössä**: Automaattinen päivitys on poistettu käytöstä.

- **Keskeytys**: järjestelmä ei ole enää oikeutettu automaattisten päivitysten vastaanottoon. Et voi määrittää tätä arvoa. järjestelmä on asettanut sen.

Lisä tietoja on kohdassa [Automaattinen päivitys](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Jos haluat ladata uusimman Azure AD Connect-version, siirry [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
