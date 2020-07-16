---
title: Yammerin käyttöoikeusongelmat
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148238"
---
# <a name="yammer-licensing-issues"></a>Yammerin käyttöoikeusongelmat

Kaikilla käyttäjillä on oltava yammer-yrityspalvelun käyttöoikeus, mutta oletusarvoisesti Yammer ei edellytä, että käyttäjillä on palvelun käyttöoikeus. Kun järjestelmänvalvoja muuttaa asetusta estääkseen Microsoft 365 -käyttäjät, joilla ei ole Yammer-käyttöoikeuksia, käyttäjät, joille ei ole määritetty Yammer Enterprise -käyttöoikeutta, eivät voi käyttää Yammer-palvelua. Lisätietoja on [ohjeaiheessa Yammer-käyttöoikeuksien hallinta Office 365:ssä](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Kun käyttöoikeudet poistetaan käyttäjiltä, Yammer-ruutua ei enää näytetä, ja muut palvelut voivat piilottaa ominaisuuksia käyttöoikeuksien poistamisen avulla. Muissa tapauksissa ominaisuudet voivat silti näkyä, mutta ne edellyttävät käyttöoikeuden myöntämistä.  

**Käyttäjän lisenssiä ei päivitetä**  

Joskus käyttäjälle on määritetty käyttöoikeus, mutta hän ei edelleenkään pysty käyttämään Yammeria. Viiveet ovat todennäköisempiä, kun joukkokäyttöoikeuden määritys on käynnissä. Yammerin käyttäjiä ei ehkä päivitetä samassa järjestyksessä kuin käyttöoikeuksia muutetaan Azure AD:ssä, koska järjestelmä toimii asynkronisesti. Odota enintään 24 tuntia ennen tukitapauksen avaamista ja ilmoita käyttöoikeuksien synkronointiongelmista.  

**Joukkolisenssin määritys**  

Käyttöoikeudet voidaan määrittää hallintakeskuksen tai PowerShell-komentosarjojen kautta. Lisätietoja on ohjeissa [Käyttöoikeuksien määrittäminen käyttäjille](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ja [Käyttöoikeuksien määrittäminen käyttäjätileille Office 365 PowerShellin avulla](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Microsoft-tuki ei tue komentosarjojen luomista, mutta Yammer-käyttöoikeusmäärityksen ohjeet ovat käytettävissä. Lisätietoja on [ohjeaiheessa Yammer-käyttöoikeuksien hallinta Windows PowerShellin avulla](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).