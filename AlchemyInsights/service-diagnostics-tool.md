---
title: Windowsin virtuaalityöpöydän palveludiagnostiikkatyökalu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595631"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Windowsin virtuaalityöpöydän palveludiagnostiikkatyökalu

Windows Virtual Desktop (WVD) tarjoaa diagnostiikkatyökalun, jonka avulla järjestelmänvalvojat voivat tunnistaa virheet yhden käyttöliittymän kautta. Tämä työkalu kirjaa diagnostiikkaan liittyvät tiedot aina, kun WVD:lle on määritetty WVD-rooli. Jokainen loki sisältää tietoja toiminnon WVD-roolista, istunnon aikana näkyviin tulemista virhesanomista sekä vuokraajan ja käyttäjän tiedot. Azure Log Analytics voidaan määrittää sieppaamaan vianmääritystyökalun luoma toimintaloki seuraavasti:

1. Luo lokianalyysin työtila [Azure-portaalin tai](https://go.microsoft.com/fwlink/?linkid=2129500) [Azure PowerShellin avulla.](https://go.microsoft.com/fwlink/?linkid=2129501)

1. [Yhdistä Windows-tietokoneet Azure Monitoriin.](https://go.microsoft.com/fwlink/?linkid=2129913) Hanki työtilan työtilan tunnus ja perusavain. Ohjattu määritystoiminto tarvitsee näitä tietoja agenttien määrittämiseen ja sen varmistamiseen, että se voi viestiä Azure Monitorin kanssa.

1. [Push diagnostiikkatiedot työtilaan.](https://go.microsoft.com/fwlink/?linkid=2128284) Voit käyttää diagnostiikkatietoja WVD-vuokraajassa työtilan lokianalyysiin.

1. [Tunnista ja diagnosoi](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) ongelmia, jotka ovat sisäisiä tai ulkoisia WVD:ssä.

Lisätietoja WVD-palvelun diagnostiikkatyökalun määrittämisestä on kohdassa Lokianalyysin käyttäminen vianmääritystoimintoa varten.