---
title: Tietoja käyttäjätiedot Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 57e7e6328747fc05b89799d631b2c6d7e0056547253aa3d75cdecb38cea3ad7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918934"
---
# <a name="about-identity-in-yammer"></a>Tietoja käyttäjätiedot Yammer

On suositeltavaa, että kaikki verkostot ottavat seuraavat toimenpiteet tunnistetietojen ongelmien välttämiseksi:

1. Pakota Office 365 käyttäjät, kun käyttäjät Microsoft 365 azure AD:ssä, jotta kaikki käyttäjät kirjautuvat sisään ensisijaisen tilin Microsoft 365 avulla. Lisätietoja on kohdassa [Käyttäjätietojen Office 365 pakote Yammer käyttäjille.](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)
2. Yhdistää useita Yammer verkostoja. Vanhat Yammer -määritykset sallivat Yammer useiden verkostojen yhteyden yhteen vuokraajaan. Lisätietoja on kohdassa Verkoston [siirto – useiden verkostojen Yammer.](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)
3. Voit halutessasi pakottaa käyttöoikeudet Yammer estää käyttäjiä Yammer, jos heillä ei ole käyttöoikeutta. Lisätietoja on kohdassa [Yammer käyttöoikeuksien hallinta Office 365.](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)
4. Valvo lopuksi vanhojen verkostojen käyttäjäluetteloa Yammer ja keskeytä vanhat käyttäjät. Käyttäjien keskeyttäminen (aktivoinnin poistaminen) on suositeltavaa niiden poistamisen sijaan, koska poistaminen on peruuttamatonta. Lisätietoja on vaihtoehdot [Käyttäjien valvonta Yammer yhteydessä](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) Office 365 ja Käyttäjien [poistaminen.](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)

Kun määrität Yammer näiden ohjeiden avulla, voit myös määrittää oman Yammer verkoston alkuperäisen tilan Microsoft 365. Lisätietoja on ohjeaiheessa [Verkkoverkon määrittäminen Yammer-tilaa varten Microsoft 365.](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode)