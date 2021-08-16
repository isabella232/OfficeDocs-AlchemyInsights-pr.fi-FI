---
title: Yammer käyttöoikeusongelmat
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
ms.openlocfilehash: 3ec764ece9cb7be933e9e2cd002379898522790528b0fa586ab501424b00cd7b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989726"
---
# <a name="yammer-licensing-issues"></a>Yammer käyttöoikeusongelmat

Kaikilla käyttäjillä on oltava Yammer Enterprise käyttöoikeus, mutta Yammer ei edellytä, että käyttäjillä on käyttöoikeus käyttää palvelua. Kun järjestelmänvalvoja estää käyttäjät, joilla Microsoft 365 ei Yammer käyttöoikeuksia, Yammer Enterprise eivät voi käyttää Yammer-palvelua. Lisätietoja on kohdassa [Käyttöoikeuksien Yammer hallinta Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Kun käyttöoikeudet poistetaan käyttäjiltä, Yammer-ruutu ei enää näy ja muut palvelut voivat käyttää käyttöoikeuden poistoa ominaisuuksien piilottaessa. Joissakin tapauksissa ominaisuudet voivat edelleen näkyä, mutta ne saattavat edellyttää lisenssien määritystä.  

**Käyttöoikeutta ei päivitetä käyttäjälle**  

Joskus käyttäjälle määritetään käyttöoikeus, mutta hän ei voi käyttää Yammer. Viiveitä ilmenee todennäköisemmin, kun joukkokäyttöoikeusmääritys on käynnissä. Yammer käyttäjiä ei ehkä päivitetä samaan järjestykseen, jossa käyttöoikeuksia muutetaan Azure AD:ssä, koska järjestelmä toimii asynkronisesti. Ilmoita käyttöoikeuksien synkronointiongelmista 24 tuntia ennen tukitapauksen avaamista.  

**Joukkolisenssien määritys**  

Käyttöoikeudet voidaan määrittää hallintakeskuksen tai PowerShell-komentosarjan kautta. Lisätietoja on tiedoissa [Käyttöoikeuksien](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) määrittäminen käyttäjille ja Käyttöoikeuksien määrittäminen [käyttäjätileille PowerShellin Office 365 avulla.](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell) 

Microsoft-tuki ei tarjoa apua komentosarjojen luomisessa, mutta käyttöoikeuksien Yammer ohjeet ovat käytettävissä. Lisätietoja on kohdassa [Käyttöoikeuksien Yammer hallinta Windows PowerShell.](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell)