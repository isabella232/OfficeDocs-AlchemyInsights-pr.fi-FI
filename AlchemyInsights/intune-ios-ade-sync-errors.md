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
ms.openlocfilehash: 1664a26b313c4a38c9c6d78cdb89997749ba175fd3dd72f278e99bbd50b0ee84
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013745"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Applen automaattisen laitteen rekisteröinnin synkronointivirheet

"Olemme havainneet, että sinulla on yksi tai useampi ADE/DEP-tunnus, joiden virhetila on. Ennen kuin kunkin tunnuksen virhetila on ratkaistu, ADE-toiminto ei toimi odotetulla tavalla.".

Tämä virhe voi ilmetä monin eri tavoin, kuten:

1. Laitteet eivät ehkä synkronoidu ABM/ASM:stä Intuneen
2. Rekisteröintiprofiilimääritykset saattavat epäonnistua
3. Laitteet eivät ehkä suorita ADE-rekisteröintiä onnistuneesti

Tarkista Intune-konsolissa ilmoitettu synkronointivirhe kohdassa Laitteet > laitteen rekisteröinti **> Apple-> rekisteröintiohjelman tunnuksia.**

Yksi synkronointivirheen yleisimpiä syitä on nykyisen tunnuksen vanheneminen. Monissa tapauksissa ongelma ratkeaa, jos tunnus on uusittava.

Jos vähintään yksi tunnuksistasi on vanhentunut, tutustu seuraaviin ohjeisiin, joiden avulla voit uusia ne tarpeen mukaan:

[Automaattisen laitteen rekisteröintitunnuksen uusiminen](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Seuraavista ohjeista näet myös muut tunnuksen synkronointivirheitä aiheuttavat virheet:

[ABM-/ASM-synkronointivirheet iOS-/iPadOS- ja macOS-laitteiden automaattisen rekisteröinnin tunnuksille](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[ABM-/ASM-synkronointivirheet iOS-/iPadOS- ja macOS-laitteiden automaattisen rekisteröinnin tunnuksille](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
