---
title: Palvelun vianmääritystyökalu Windows virtuaalityöpöydälle
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
ms.openlocfilehash: 58688e3216ba6777b1a4f76095bd39c81a2d2a8294e06b6bc61c7134f6d589f9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052383"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Palvelun vianmääritystyökalu Windows virtuaalityöpöydälle

Windows Virtual Desktop (WVD) on diagnostiikkatyökalu, jonka avulla järjestelmänvalvojat voivat tunnistaa virheitä yhden liittymän kautta. Tämä työkalu kirjaa diagnostiikkaan liittyvät tiedot aina, kun WVD:lle on määritetty WVD-rooli. Jokainen loki sisältää tietoja toiminnon WVD-roolista, istunnon aikana näkyviin tulemista virhesanomista sekä vuokraajan ja käyttäjän tiedot. Azure Log Analytics voidaan määrittää sieppaamaan vianmääritystyökalun luoma toimintaloki. Toimi seuraavasti:

1. Luo Lokianalyysi-työtila [Azure-portaalin tai](https://go.microsoft.com/fwlink/?linkid=2129500) [Azure PowerShellin avulla.](https://go.microsoft.com/fwlink/?linkid=2129501)
1. [Näyttöyhteys Windows Azure Monitoriin.](https://go.microsoft.com/fwlink/?linkid=2129913) Hanki työtilan tunnus ja perusavain. Ohjattu määritystoiminto tarvitsee näitä tietoja, jotta agentti voidaan määrittää oikein ja jotta se voi viestiä Azure Monitorin kanssa.
1. [Push diagnostiikkatiedot työtilaan.](https://go.microsoft.com/fwlink/?linkid=2128284) Voit käyttää diagnostiikkatietoja WVD-vuokraajassa työtilan lokianalyysiin.
1. [Tunnista ja diagnosoi](https://go.microsoft.com/fwlink/?linkid=2128338) ongelmia, jotka ovat sisäisiä tai ulkoisia WVD:tä varten.

Lisätietoja WVD:n palvelun diagnostiikkatyökalun määrittämisestä on kohdassa [Lokianalyysin käyttäminen vianmääritystoimintoa varten.](https://go.microsoft.com/fwlink/?linkid=2128084)
