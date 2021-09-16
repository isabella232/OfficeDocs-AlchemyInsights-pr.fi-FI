---
title: Microsoft 365 -hallintakeskuksen raportit eivät näytä luettavaa käyttäjänimeä
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13809"
- "13810"
- "13812"
- "9008619"
ms.openlocfilehash: ff8eac6487ef544277c5ce2c0c0b7068c9d400ca
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2021
ms.locfileid: "59327811"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Microsoft 365 -hallintakeskuksen raportit eivät näytä luettavaa käyttäjänimeä

Microsoft 365 -hallintakeskuksen raportit eivät näytä käyttäjänimiä vaan aakkosnumeerisia arvoja, kuten B2BC6C15BB9FCDEA71E5CD302D228CC8.

Tämä on odotettua toimintaa, josta on ilmoitettu Viestikeskuksen kautta (MC275344, julkaistu 3. elokuuta 2021). 

Yleiset järjestelmänvalvojat voivat palauttaa tämän muutoksen vuokraajassaan ja näyttää tunnistettavia käyttäjätietoja, jos organisaation tietosuojakäytännöt niin sallivat. Voit palauttaa muutoksen vuokraajassa seuraavasti:

1. Siirry hallintakeskuksessa kohtaan **Asetukset** > **Organisaation asetukset** > [**Palvelut**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services ) ja valitse **Raportit**. 
1. Valitse kohdassa **Valitse, miten käyttäjätiedot näytetään** asetus **Näytä tunnistettavissa olevat käyttäjätiedot raporteissa** ja suorita sitten raportti uudelleen.