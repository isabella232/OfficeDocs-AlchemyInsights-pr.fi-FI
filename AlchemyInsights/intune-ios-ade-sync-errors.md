---
title: Applen automaattisen laitteen rekisteröinnin synkronointivirheet
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448919"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Applen automaattisen laitteen rekisteröinnin synkronointivirheet

"Olemme havainneet, että sinulla on yksi tai useampi ADE/DEP-tunnus, joka on virhetilassa. Ennen kuin virhetila on ratkaistu kunkin tunnuksen osalta, ADE-toiminto ei toimi odotetulla tavalla."

Tämä virhe voi ilmetä monin eri tavoin, kuten:

1. Laitteet eivät ehkä synkronoidu ABM/ASM:stä Intuneen
2. Rekisteröintiprofiilimääritykset saattavat epäonnistua
3. Laitteet eivät ehkä suorita ADE-rekisteröintiä onnistuneesti

Tarkista Intune-konsolissa ilmoitettu synkronointivirhe Laitteet-kohdassa, > rekisteröi laitteet **> Apple-rekisteröinti>-ohjelman tunnukset.**

Yksi yleisimmistä synkronointivirheen syistä on nykyisen tunnuksen vanheneminen. Monissa tapauksissa ongelma ratkeaa, jos kyseinen tunnus uusitaan.

Jos vähintään yksi tunnuksesi on vanhentunut, tutustu seuraaviin ohjeisiin, joiden avulla voit uusia ne tarpeen mukaan:

[Automaattisen laitteen rekisteröintitunnuksen uusiminen](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Lisäksi seuraavista ohjeista näet mahdolliset korjaaminen muista virheistä, jotka aiheuttavat tunnusten synkronointivirheitä:

[ABM-/ASM-synkronointivirheet iOS-/iPadOS- ja macOS-laitteiden automaattisen rekisteröinnin tunnuksille](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[ABM-/ASM-synkronointivirheet iOS-/iPadOS- ja macOS-laitteiden automaattisen rekisteröinnin tunnuksille](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
