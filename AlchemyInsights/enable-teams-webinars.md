---
title: Verkkoseinaarien Teams ottaminen käyttöön
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793650"
---
# <a name="enable-teams-webinars"></a>Verkkoseinaarien Teams ottaminen käyttöön

Webinaarit ovat oletusarvoisesti käytössä. Voit hallita sitä, kuka voi ajoittaa ja rekisteröidä Teams Webinaarit-Teams PowerShell-komennoilla.

- Kaikki käyttäjät, jotka voivat luoda kokouksen, voivat myös luoda webinaarikokouksen. Jos haluat hallita sitä, kuka voi Teams Webinaarit, käytä *AllowMeetingRegistration-sovellusta.* 
- *Oletusarvoisesti WhoCanRegister* on käytössä ja sen asetuksena on **Kaikki.** Jos haluat poistaa kokouksen rekisteröinnin käytöstä, määritä *AllowMeetingRegistration-asetuksen arvoksi* **Epätosi.**

Jos haluat muuttaa näitä asetuksia, sinun on asennettava [Teams PowerShell.](/microsoftteams/teams-powershell-install) Kokouskäytännöt ovat myös käytössä Teams webinaarissa. Jos esimerkiksi anonyymi liittyminen on poistettu käytöstä kokousasetuksissa, anonyymit käyttäjät eivät voi liittyä webinaariin.

Lisätietoja sen määrittämisestä, kuka voi rekisteröityä webinaariin, on kohdassa Määritä, [kuka voi rekisteröityä webinaariin.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars) Lisätietoja Microsoft-luetteloiden asetuksista on artikkelissa [Microsoft-luetteloiden asetusten hallinta.](/sharepoint/control-lists)