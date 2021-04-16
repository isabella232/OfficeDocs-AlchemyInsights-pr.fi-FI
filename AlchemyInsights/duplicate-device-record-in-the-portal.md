---
title: Laitetietueen kaksoiskappale portaalissa
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814513"
---
# <a name="duplicate-device-record-in-the-portal"></a>Laitetietueen kaksoiskappale portaalissa

Laitteelle voi olla portaalissa näkyvissä 2 tietuetta, jos laite ei ilmoita oikein yhteishallintatilaa Configuration Manager -sivustolle. Jos haluat tarkistaa laitteen yhteishallintatilan, katso laitteen **Yhteishallinta**-sarake Configuration Manager -konsolista. Jos sarake ei ole näkyvissä, voit lisätä sen napsauttamalla jotakin sarakkeen otsikoista hiiren kakkospainikkeella ja valitsemalla sen luettelosta.

Yhteishallinta-arvon pitää olla **Kyllä**. Jos arvo on **Ei**, avaa Configuration Manager -asiakassovellus asiakaslaitteesta ja tarkista **Yhteishallinta**-ominaisuus Yleiset-välilehdeltä.

- Jos arvo on **Käytössä**, tämä tarkoittaa ongelmia asiakasviestinnässä hallintapisteissä. Tarkista laitteen **CcmMessaging. log** mahdollisten yhteysongelmien tutkimiseksi.

- Jos arvo on **Pois käytöstä** ja laite on rekisteröity Intunessa, varmista, että laite on saanut yhteishallintakäytännön tarkistamalla laitteesta lokin **CoManagementHandler.log**.
