---
title: Dynamics 365-väärä koonti näyttö näytetään Dynamics 365 Unified Interface-liittymässä
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711272"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Väärä koonti näyttö näytetään Dynamics 365 Unified Interface-liittymässä

On useita syitä siihen, miksi näyttöön voi tulla jokin muu koonti näyttö kuin odotit:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Käyttäjä on määrittänyt käyttäjän oletus koonti näytön 

Yleensä käyttäjä voi määrittää oletus koonti näytön, jos **Määritä oletukseksi** -painike ei näy koonti näytön komento palkissa. Käyttäjän oletus koonti näyttö ohittaa kaikki muut oletusarvoiset raportti näkymät, vaikka käyttäjän oletus koonti näyttö ei olisi nykyisessä sovelluksessa.

Voit poistaa oletus koonti näytön käytöstä noudattamalla seuraavia vaihto ehtoista vaihto ehtoista menetelmää.

1. Luo uusi henkilökohtainen koonti näyttö.

2. Uuden koonti näytön määrittäminen käyttäjän oletukseksi.

3. Poista raportti näkymä.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Koonti näyttö määritetään sivustokarttaan

Olet ehkä määrittänyt organisaation oletus koonti näytön valitsemalla koonti näytön ja valitsemalla "Määritä oletukseksi" kohdassa "Mukauta järjestelmää". Sivustokartta Designerissa määritetty koonti näyttö ohittaa tämän koonti näytön, jos käyttäjä voi käyttää sitä.

Jos haluat, että käyttäjät näkevät koonti näytön, jonka olet määrittänyt organisaation oletukseksi, voit joko:

* Näyttö näkymän asettaminen sivustokarttaan

* Sivustokartan käyttö oikeuden poistaminen määritettyjen käyttäjien koonti näytöstä
