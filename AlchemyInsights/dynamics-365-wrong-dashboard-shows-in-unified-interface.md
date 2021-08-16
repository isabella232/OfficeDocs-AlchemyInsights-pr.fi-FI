---
title: Dynamics 365 – Väärä raporttinäkymä näkyy Dynamics 365:n yhdistetyssä käyttöliittymässä
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
ms.openlocfilehash: 1edb2a7e9e0c270c7e98eb43d2f6514d70c39a19ea97d189322ca387b6842a18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101479"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Väärä koontinäyttö näkyy Dynamics 365:n yhdistetyssä käyttöliittymässä

On useita syitä siihen, miksi saatat nähdä eri koontinäytön kuin oletit:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Käyttäjä on määrittänyt käyttäjän oletuskoontinäytön 

Voit yleensä määrittää käyttäjän oletuskoontinäytön, jos Aseta **oletukseksi** -painike ei näy koontinäytön komentopalkissa. Käyttäjän oletuskoontinäyttö ohittaa kaikki muut oletusarvoiset koontinäytöt, vaikka käyttäjän oletuskoontinäyttö ei olisi nykyisessä sovelluksessa.

Voit poistaa oletuskoontinäytön joukon seuraavasti:

1. Luo uusi henkilökohtainen koontinäyttö.

2. Määritä uusi koontinäyttö käyttäjän oletusnäkymäksi.

3. Poista raporttinäkymä.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Koontinäyttö on määritetty sivustokartassa

Olet ehkä määrittänyt organisaation oletuskoontinäytön valitsemalla koontinäytön ja valitsemalla Mukauta järjestelmää -kohdassa Aseta oletukseksi. Sivustokartan suunnittelussa määritetty koontinäyttö on kuitenkin etusijalla, jos käyttäjällä on sen käyttöoikeus.

Jos haluat, että käyttäjät näkevät koontinäytön, jonka olet määrittänyt organisaation oletusnäkymäksi, voit tehdä jommankumman seuraavista:

* Raporttinäkymän määrittäminen sivustokartassa

* Kyseisten käyttäjien sivustokarttaan määritetyn koontinäytön näkymän näkymän poistaminen
