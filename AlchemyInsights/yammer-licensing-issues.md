---
title: Yammer-käyttö oikeus ongelmat
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657273"
---
# <a name="yammer-licensing-issues"></a>Yammer-käyttö oikeus ongelmat

Kaikilla käyttäjillä on oltava käyttö oikeus Yammer Enterprise-palvelun käyttöön, mutta oletusarvoisesti Yammer ei edellytä, että käyttäjillä on oikeus käyttää palvelua. Kun järjestelmänvalvoja muuttaa asetusta niin, että se estää Microsoft 365-käyttäjät, joilla ei ole Yammer-käyttö oikeuksia, Yammer Enterprise-käyttö oikeutta ei voi käyttää. Lisä tietoja on Ohje aiheessa [Yammer-käyttö oikeuksien hallinta Office 365-](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) sovelluksessa 

Kun käyttö oikeuksia poistetaan käyttäjiltä, Yammer-ruutu ei ole enää näkyvissä ja muut palvelut voivat piilottaa ominaisuuksia käyttö oikeuksien poistamisen avulla. Muissa tapa uksissa ominaisuudet voivat edelleen näkyä, mutta ne edellyttävät, että käyttö oikeus määritystä käytetään.  

**Käyttäjä ei saa päivitettyä käyttö oikeutta**  

Toisinaan käyttäjälle määritetään käyttö oikeus, mutta se ei edelleenkään pysty käyttämään Yammeria. Viiveet tapahtuvat todennäköisemmin, kun massa käyttö oikeuden määritys on käynnissä. Yammer-käyttäjiä ei ehkä päivitetä samassa järjestyksessä kuin käyttö oikeuksia muutetaan Azure AD:ssä, koska järjestelmä suoritetaan asynkronisesti. Odota 24 tuntia, ennen kuin avaat tuki tapauksen ja ilmoitat käyttö oikeuksien synkronoinnin ongelmista.  

**Bulk todistus-määritys**  

Käyttö oikeudet voidaan määrittää hallinta keskuksen tai PowerShell-komento sarjojen kautta. Lisä tietoja on Ohje aiheissa [käyttö oikeuksien määrittäminen käyttäjille](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ja käyttö [oikeuksien määrittäminen käyttäjä tileille Office 365 PowerShellin avulla](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Microsoft-tuki ei anna ohjeita komento sarjojen luomiseen, mutta ohjeet ovat käytettävissä Yammer-käyttö oikeuksien määritystä varten. Lisä tietoja on Ohje aiheessa [Yammer-käyttö oikeuksien hallinta Windows PowerShellin avulla](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).