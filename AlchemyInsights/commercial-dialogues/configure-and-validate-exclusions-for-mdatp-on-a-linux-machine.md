---
title: MDATP-poikkeuksien määrittäminen ja vahvistaminen Linux-koneessa
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
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746025"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a>MDATP-poikkeuksien määrittäminen ja vahvistaminen Linux-koneessa

Voit jättää tietyt tiedostot, kansiot, prosessit ja prosessi avatut tiedostot pois MDATP-skannauksista. Poikkeukset auttavat estämään ohjelmistojen ja tiedostojen virheellisen tunnistuksen, joka on yksilöllinen tai mukautettu organisaatiollesi. Poikkeukset auttavat myös MDATP:n aiheuttamien suorituskykyongelmien lieventämiseen.

Lisätietoja on kohdassa [MDATP for Linuxin poikkeusten](https://go.microsoft.com/fwlink/?linkid=2144517)määrittäminen ja vahvistaminen.

> [!IMPORTANT]
> Tässä artikkelissa kuvatut poikkeukset eivät koske muita MDATP for Linuxin ominaisuuksia, kuten päätepisteiden tunnistusta ja vastausta. Tässä artikkelissa kuvattujen menetelmien avulla ohitettavat tiedostot voivat silti käynnistää EDR-ilmoituksia ja muita tunnistusominaisuuksia.
