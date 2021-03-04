---
title: Tietojen ja laitteiden poistaminen Intunesta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416310"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Tietojen ja laitteiden poistaminen Intunesta

Laitteen käytöstä poistaminen ja laitteen tietojen poistaminen ovat etätoimintoja, joilla voidaan poistaa Intunen hallitsemia yritystietoja tai suorittaa tehdasasetusten palautus ja palauttaa laitteen oletusasetukset.

1. Kirjaudu sisään Microsoft 365 -laitteiden hallintaan ja siirry kohtaan **Laitteet** > **Kaikki laitteet**.
2. Valitse laite, jonka tiedot haluat poistaa.
3. Valitse, minkä tyyppistä etäpoistoa haluat käyttää. Laitteen käytöstä poistaminen poistaa vain yrityksen tiedot, kun taas kaikkien tietojen poistaminen palauttaa laitteen tehdasasetukset.
4. Vahvista valitsemalla **Kyllä**. Kunnes tietojen poistaminen on valmis, laitteen toiminnon tila näyttää, että *Käytöstä poisto odottaa*.
    Kun toiminto on valmis, mobiililaite ei näy enää hallittujen laitteiden listassa.

> [!NOTE]
> Yritystietoja ei voi poistaa laitteista, jotka on LIITETTY Azure AD:hen. 

Lisätietoja laitteen käytöstä poistamisen ja laitteen tietojen poistamisen vaikutuksista, mukaan lukien siitä, mitä säilytetään ja mitä poistetaan, löytyy seuraavista ohjeista:

- [Poista laite poistamalla se käytöstä, poistamalla laitteen tiedot tai poistamalla laitteen rekisteröinti manuaalisesti](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).
- [Kuinka poistaa vain yritystiedot Intunen hallitsemista sovelluksista](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Poista kaikki tiedot macOS-laitteesta](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).