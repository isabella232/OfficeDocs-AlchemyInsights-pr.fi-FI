---
title: Windowsin Näennäistyöpöytä-palvelun diagnostiikka työkalu
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/14/2020
ms.locfileid: "49678620"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Windowsin Näennäistyöpöytä-palvelun diagnostiikka työkalu

Windowsin Näennäistyöpöytä (WVD) tarjoaa diagnostiikka työkalun, jonka avulla järjestelmänvalvojat tunnistavat virheet yksittäisen liittymän kautta. Tämä työkalu kirjaa diagnostiikkaan liittyviä tietoja aina, kun WVD käyttää WVD-roolia. Jokainen loki sisältää tietoja toiminnon WVD-roolista, istunnon aikana ilmestymis virhe sanomista sekä vuokra ajan ja käyttäjän tiedoista. Azure log Analyticsin voi määrittää tallentamaan diagnostiikka työkalun luoman toiminta loki tiedot. Toimi seuraavasti:

1. Luo loki analytiikka-työtila [Azure-portaalissa](https://go.microsoft.com/fwlink/?linkid=2129500) tai [Azure PowerShellissä](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [Yhdistä Windows-tieto koneet Azure Monitoreen](https://go.microsoft.com/fwlink/?linkid=2129913). Hanki työtilan tunnus ja työtilan perusavain. Ohjattu määritys toiminto tarvitsee näitä tietoja, jotta agentti voidaan määrittää oikein ja jotta se voi kommunikoida Azure monitorissa.
1. [Paina diagnostiikan tiedot työtilaan](https://go.microsoft.com/fwlink/?linkid=2128284). Voit siirtää diagnostiikan tietoja WVD-vuokra ajasta työtilan loki analytiikkaan.
1. [Tunnista ja diagnosoimaan ongelmia](https://go.microsoft.com/fwlink/?linkid=2128338) , jotka ovat sisäisiä tai ulkoisia suhteessa WVD.

Lisä tietoja WVD-palvelun vian määritys työkalun määrittämisestä on artikkelissa [loki analyysin käyttäminen Diagnostiikka-toimintoa varten](https://go.microsoft.com/fwlink/?linkid=2128084).
