---
title: Puhelun tallentaminen 1:1
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
ms.openlocfilehash: 8cdadf34a059856338d7f40528446b70373465e4
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702087"
---
# <a name="11-call-recording"></a>Puhelun tallentaminen 1:1

Jos Aloita **tallennus -painike** näkyy harmaana yhden puhelun aikana, sinun on muutettava käyttäjän käytäntöasetuksia. Voit tarkistaa käytäntöasetuksen ajamalla vianmäärityksen käyttäjälle kirjoittamalla **yllä Diag: Teams 1:1 -puhelutallenteen.**     

31. toukokuuta 2021 alkaen otamme käyttöön uuden puhelukäytännön *AllowCloudRecordingForCalls Teams* käyttöön. Ennen tätä muutosta 1:1-puhelutallenteen hallinnassa on *AllowCloudRecording* Teams kokouskäytäntö. Tämä muutos on dokumentoitu viestikeskuksen viestissä: [(Päivitetty) 1:1 Puhelutallennuskäytännön esittely](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).  

*AllowCloudRecordingForCalls*   puhelukäytäntöasetus on **$False** oletusarvoisesti. Jos haluat estää kaikkia käyttäjiä nauhoittamaan 1:1-puheluita, sinun ei tarvitse tehdä mitään.  

Jos haluat ottaa puhelutallenteen käyttöön kaikille käyttäjille 1:1-puheluissa, [suorita Teams cmdlet-komento PowerShellin](/microsoftteams/teams-powershell-install) avulla: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Vaihtoehtoisesti voit luoda uuden käytännön ja määrittää **AllowCloudRecordingForCalls** -$true **ja** määrittää käytännön käyttäjille. 

Lisätietoja on kohdassa [1:1 Puhelun tallennuskäytännön ohjausobjektit ovat (lähes!) Täällä](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
