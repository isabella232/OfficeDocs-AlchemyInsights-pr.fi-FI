---
title: OneDriven Kirjautumisvirhe AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982449"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDriven Kirjautumisvirhe AADSTS50011

Jos näyttöön tulee virhe ilmoitus "AADSTS50011: Pyynnössä määritetty vasta uksen URL-osoite ei vastaa vastausta" kun kirja udut sisään OneDrive-sovellukseen, tarkista seuraavat asiat:

OneDrive-versiosi on oltava yhtä suuri tai suurempi kuin versio 20.052. XXXX. XXXX. Jos haluat tarkistaa versiosi, napsauta ilmaisin alueella olevaa sinistä OneDrive-kuvaketta ja valitse **ohje & asetukset > asetukset > tietoja**.

Verkostosi voi estää liikennettä **g.live.com** ja **oneclient.SFX.MS**. Jos liikenne on estynyt, OneDrive ei voi päivittää itseään. Varmista verkonvalvojan kanssa, että sinulla on näiden URL-osoitteiden käyttäminen. [Näiden pääte pisteiden](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) pitäisi olla tavoitettavissa asiakkaille, jotka käyttävät Microsoft 365-palvelu pakettia.

Jos haluat hankkia OneDriven nykyisen version manuaalisesti, käy [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
