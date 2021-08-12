---
title: MDATP-ohittamisen määrittäminen ja vahvistaminen Linux-koneessa
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 96579b28923e392a0fa05c56833fed1b45eb118437ac7e8333c610ed69126f8e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53916412"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a>MDATP-ohittamisen määrittäminen ja vahvistaminen Linux-koneessa

Voit jättää tietyt tiedostot, kansiot, prosessit ja prosessi avatut tiedostot MDATP-tarkistusten ulkopuolelle. Poikkeukset auttavat estämään ohjelmistojen ja tiedostojen virheellisen tunnistamisen, joka on yksilöity tai mukautettu organisaatiotasi varten. Poikkeukset auttavat myös MDATP:n aiheuttamien suorituskykyongelmien lieventämiseen.

Lisätietoja on kohdassa [MDATP-protokollan poikkeuksien määrittäminen ja vahvistaminen Linuxissa.](https://go.microsoft.com/fwlink/?linkid=2144517)

> [!IMPORTANT]
> Tässä artikkelissa kuvatut poikkeukset eivät koske muita MDATP for Linuxin ominaisuuksia, kuten päätepisteiden tunnistus ja käsittely (päätepisteiden tunnistus ja käsittely). Tässä artikkelissa kuvattujen menetelmien avulla pois jätettävät tiedostot voivat silti käynnistää päätepisteiden tunnistus ja käsittely ja muita tunnistusominaisuuksia.
