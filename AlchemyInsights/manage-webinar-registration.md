---
title: Verkkoseinaarin rekisteröinnin hallinta
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
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793708"
---
# <a name="manage-webinar-registration"></a>Verkkoseinaarin rekisteröinnin hallinta

Voit hallita sitä, kuka voi rekisteröityä Teams Webinaarit-Teams PowerShell-komennoilla. Jos haluat asentaa Teams PowerShellin, katso [Teams PowerShelliä.](/microsoftteams/teams-powershell-install) 

*Oletusarvoisesti WhoCanRegister* on käytössä ja sen asetuksena **on EveryoneInCompany.** Jotta kuka tahansa, anonyymit käyttäjät mukaan lukien, voi  rekisteröityä, sinun on määritettävä kokouskäytännön arvoksi Kaikki PowerShell-komennolla:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Huomautus:** Jos anonyymi liittyminen on poistettu käytöstä kokousasetuksissa, anonyymit käyttäjät eivät voi liittyä webinaariin. Lisätietoja ja tämän asetuksen käyttöönotto on kohdassa [Kokousasetusten hallinta Microsoft Teams.](/microsoftteams/meeting-settings-in-teams)

Jos haluat poistaa kokouksen rekisteröinnin käytöstä, määritä *AllowMeetingRegistration-asetuksen arvoksi* **Epätosi.**

Lisätietoja sen määrittämisestä, kuka voi rekisteröityä webinaariin, on kohdassa Määritä, [kuka voi rekisteröityä webinaariin.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars) Lisätietoja Microsoft-luetteloiden asetuksista on artikkelissa [Microsoft-luetteloiden asetusten hallinta.](/sharepoint/control-lists)
