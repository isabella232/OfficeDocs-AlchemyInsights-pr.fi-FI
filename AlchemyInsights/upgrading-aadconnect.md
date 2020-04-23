---
title: 932 AADConnectin päivittäminen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766490"
---
# <a name="upgrade-azure-ad-connect"></a>Azure AD Connectin päivittäminen

Oletusarvon mukaan automaattinen päivitys on käytössä Azure AD Connectissa, mikä auttaa varmistamaan, että käytössäsi on uusin versio. Voit tarkistaa automaattiset päivitysasetukset Azure AD PowerShellin **Get-ADSyncAutoUpgrade-cmdlet-komentoa** käyttämällä. Cmdlet palauttaa jonkin seuraavista arvoista:

- **Käytössä:** Automaattinen päivitys on käytössä.

- **Ei käytössä**: Automaattinen päivitys on poistettu käytöstä.

- **Keskeytetty:** Järjestelmä ei ole enää oikeutettu vastaanottamaan automaattisia päivityksiä. Tätä arvoa ei voi määrittää. Se on asetettu järjestelmä.

Lisätietoja on kohdassa [Automaattinen päivitys](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Jos haluat ladata Azure AD Connectin [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)uusimman version, siirry kohtaan .
