---
title: OneDrive kirjautumisvirhe AADSTS50011
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
ms.openlocfilehash: 80aafa2aee7213e1b77d274509a7eb9741c20b525ed97f473093ac8c6514f3c7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54112909"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive kirjautumisvirhe AADSTS50011

Jos saat virhesanoman "AADSTS50011: Pyynnössä määritetty url-osoite ei vastaa vastausta", kun kirjaudut OneDrive-sovellukseen, tarkista seuraavat asiat:

Oman OneDrive on oltava vähintään 20.052.XXXX.XXXX-versiota suurempi. Voit tarkistaa versiosi napsauttamalla ilmaisinalueen OneDrive-kuvaketta ja valitsemalla **Ohje-& Asetukset > Asetukset > Tietoja**.

Verkko saattaa estää liikenteen g.live.com  **oneclient.sfx.ms.** Jos tämä liikenne on estetty, OneDrive ei voi päivittää itse. Varmista verkon järjestelmänvalvojan kanssa, että voit käyttää näitä URL-osoitteita. [Näiden päätepisteiden pitäisi](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) olla Microsoft 365.

Jos haluat manuaalisesti saada nykyisen OneDrive, siirry [https://aka.ms/getonedrive](https://aka.ms/getonedrive) kohteeseen.
