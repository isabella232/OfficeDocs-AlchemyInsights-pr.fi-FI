---
title: Laitetietueen kaksoiskappale portaalissa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2020
ms.locfileid: "43789859"
---
# <a name="duplicate-device-record-in-the-portal"></a>Laitetietueen kaksoiskappale portaalissa

Laitteelle voi olla portaalissa näkyvissä 2 tietuetta, jos laite ei ilmoita oikein yhteishallintatilaa Configuration Manager -sivustolle. Jos haluat tarkistaa laitteen yhteishallintatilan, katso laitteen **Yhteishallinta**-sarake Configuration Manager -konsolista. Jos sarake ei ole näkyvissä, voit lisätä sen napsauttamalla jotakin sarakkeen otsikoista hiiren kakkospainikkeella ja valitsemalla sen luettelosta.

Yhteishallinta-arvon pitää olla **Kyllä**. Jos arvo on **Ei**, avaa Configuration Manager -asiakassovellus asiakaslaitteesta ja tarkista **Yhteishallinta**-ominaisuus Yleiset-välilehdeltä.

- Jos arvo on **Käytössä**, tämä tarkoittaa ongelmia asiakasviestinnässä hallintapisteissä. Tarkista laitteen**CcmMessaging. log** mahdollisten yhteysongelmien tutkimiseksi.

- Jos arvo on **Pois käytöstä** ja laite on rekisteröity Intunessa, varmista, että laite on saanut yhteishallintakäytännön tarkistamalla laitteesta lokin**CoManagementHandler.log**.
