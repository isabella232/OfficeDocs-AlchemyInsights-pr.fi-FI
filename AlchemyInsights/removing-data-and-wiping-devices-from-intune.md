---
title: Tietojen poistaminen ja laitteiden pyyhkiminen Intunesta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439650"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Tietojen poistaminen ja laitteiden pyyhkiminen Intunesta

Device Retire- ja Device Wipe -etätoimintoja voidaan käyttää Intune-järjestelmän hallinnoimien yritystietojen poistamiseen tai tehdasasetusten palauttamiseen ja laitteen oletusasetusten palauttamiseen.

1. Kirjaudu Microsoft 365 Device Managementiin ja valitse **Laitteet**  >  **kaikki laitteet**.
2. Valitse laite, jonka haluat pyyhkiä.
3. Valitse etätyhjennuksen tyyppi, jonka haluat tehdä. Poista käytöstä vain organisaatiotiedot, kun taas täydet pyyhkeet palauttavat laitteen tehdasasetuksiinsa.
4. Vahvista valitsemalla **Kyllä.** Laitetoiminnon tila näkyy Odottavassa tilassa, kunnes pyyhi on valmis.</br>
    Kun toiminto on valmis, et enää näe mobiililaitetta hallitun laitteen luettelossa.

**Huomautus** Yrityksen tietoja ei voi poistaa Azure AD:hen liitetyistä laitteista.

Täydelliset tiedot Käytöstä- ja Pyyhi-toimintojen vaikutuksesta, mukaan lukien säilytetyt ja poistetut toiminnot, on [ohjeaiheessa Laitteiden poistaminen pyyhkimällä, poistamalla käytöstä tai poistamalla laitteen manuaalisesti](https://docs.microsoft.com/intune/devices-wipe).

Lisätietoja kaikkien tietojen poistamisesta macOS-laitteesta on [ohjeaiheessa Kaikkien tietojen poistaminen macOS-laitteesta](https://docs.microsoft.com/intune/device-erase).