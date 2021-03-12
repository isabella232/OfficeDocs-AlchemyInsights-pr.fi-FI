---
title: 1:1-puhelutallenne
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733846"
---
# <a name="11-call-recording"></a>1:1-puhelutallenne

Järjestelmänvalvojien on nyt jatkettava 1:1-puheluiden tallentamista.
 
12. huhtikuuta 2021 alkaen otamme käyttöön uuden Teams-puhelukäytäntövaihtoehdon *AllowCloudRecordingForCalls.* 

Tällä hetkellä yhden puhelun tallennusominaisuuksia hallitaan Teamsin *kokouskäytäntöjen AllowCloudRecording-vaihtoehdolla.* Jos käyttäjät voivat tallentaa Teams-kokouksia, he voivat myös tallentaa 1:1-puheluita.

Jos haluat estää kaikkia käyttäjiä nauhoittamaan 1:1-puheluita, sinun ei tarvitse tehdä mitään. *AllowCloudRecordingForCalls-puhelukäytäntöasetus* $False oletusarvoisesti.

Tämä muutos on dokumentoitu seuraavassa viestikeskuksen viestissä: [(Päivitetty) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) Puhelun tallennuskäytännön esittely Teams-puhelukäytäntövaihtoehdon valitsemiseen on käytettävä [Teams PowerShelliä.](https://docs.microsoft.com/microsoftteams/teams-powershell-install)

**Puhelutallenteen ottaminen käyttöön 1:1-puheluissa:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True

**Puhelun tallennuksen poistaminen käytöstä 1:1-puheluissa:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False

