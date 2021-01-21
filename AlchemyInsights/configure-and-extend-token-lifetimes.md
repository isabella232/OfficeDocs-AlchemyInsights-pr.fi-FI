---
title: Tunnusten elinkaaren määrittäminen ja pidentäminen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916825"
---
# <a name="configure-and-extend-token-lifetimes"></a>Tunnusten elinkaaren määrittäminen ja pidentäminen

Voit määrittää Microsoftin tunnistetietoympäristön myöntämien käytön, SAML-tunnusten tai tunnustietueiden elinkaaren. Voit määrittää tunnuksen elinkaaren kaikille organisaation sovelluksille, usean vuokraajan (usean organisaation) sovellukselle tai tietylle organisaation palvelun päätasolle. Lisätietoja on lukukelpoisissa [tunnusten käyttöiän määrittämisessä.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)

Esimerkkejä tunnusten elinkaaren määrittämisestä on [esimerkeissä.](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes)

Lisätietoja tunnuksen elinkaaren ja yhteensopivuuden määrittämisestä Azure Active Directory B2C:ssä (Azure AD B2C) on kohdassa Tunnusten määrittäminen [Azure Active Directory B2C:ssä.](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow)

Artikkelissa Määritä istunnon toiminta [Azure Active Directory B2C:ssä](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) kuvataan Azure AD B2C:ssä käytettävät kertakirjautumismenetelmät ja sen avulla voit valita sopivimman kertakirjautumismenetelmän käytäntöä määritettäessä.

**Kuinka kauan tunnukset kestävät? Kuinka kauan ne ovat voimassa?**

Tunnusten käyttöajat ovat 1 tunti ja istunnon elinaika on 24 tuntia. Tämä tarkoittaa, että jos pyyntöjä ei ole tehty 24 tunnin kuluessa, sinun on kirjauduttava uudelleen sisään ennen uuden tunnuksen pyytämista.

> [!NOTE]
> 30. toukokuuta 2020 jälkeen kukaan uusi vuokraaja ei voi käyttää Määritettävissä olevan tunnusten elinkaari -käytäntöä istuntojen ja päivitystunnusten määrittämiseen. Poisto tapahtuu useiden kuukausien kuluessa, mikä tarkoittaa, että lopetamme nykyisen istunnon ja päivitämme tunnusten tunnukset. Voit edelleen määrittää käyttöoikeustietueen elinkaaren poiston jälkeen.






