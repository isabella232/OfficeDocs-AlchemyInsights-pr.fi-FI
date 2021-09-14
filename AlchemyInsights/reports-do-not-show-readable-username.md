---
title: Raportit Microsoft 365 -hallintakeskus eivät näytä luettavissa olevia käyttäjänimiä
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
ms.openlocfilehash: 16aa4f052c934421423c73244f03a20aa38e4785
ms.sourcegitcommit: 76c61dec041b93d0039764fae38107108da324aa
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/04/2021
ms.locfileid: "59315984"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Raportit Microsoft 365 -hallintakeskus eivät näytä luettavissa olevia käyttäjänimiä

Raportit Microsoft 365 -hallintakeskus näytä käyttäjänimiä, vaan näyttävät aakkosnumeeriset arvot, kuten B2BC6C15BB9FCDEA71E5CD302D228CC8.

Tämä on odotettavissa, ja siitä on ilmoitettu viestikeskuksessa (MC275344, julkaistu 3. elokuuta 2021). 

Yleiset järjestelmänvalvojat voivat palauttaa tämän muutoksen vuokraajassaan ja näyttää tunnistettavia käyttäjätietoja, jos heidän organisaation tietosuojakäytäntönsä sallivat. Vuokraajan muutoksen muuttaminen:

1. Siirry hallintakeskuksessa kohtaan Organisaation **Asetukset**  >    >  [**Palvelut**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services)ja valitse **Raportit**. 
1. Valitse **Valitse käyttäjätietojen näyttäminen -kohdassa** **Näytä tunnistettavissa olevat käyttäjätiedot raporteissa** ja suorita raportti uudelleen.