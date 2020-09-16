---
title: Tietoja tunniste tiedoista Yammerissa
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
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664167"
---
# <a name="about-identity-in-yammer"></a>Tietoja tunniste tiedoista Yammerissa

On suositeltavaa, että kaikki verkot seuraavat vaiheita, jotta identiteettiin liittyviä ongelmia voidaan välttää:

1. Pane täytäntöön Office 365-käyttäjä tiedot, kun Microsoft 365-tilit on luotu Azure AD:ssä, jotta kaikki käyttäjät voivat kirja utua sisään käyttämällä ensisijaisia Microsoft 365-tilejään. Lisä tietoja on Ohje aiheessa [Office 365-käyttäjä tietojen määrittäminen Yammer-käyttäjille](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Useiden Yammer-verkostojen kokoaminen. Aiemmat Yammer-määritykset sallivat useiden Yammer-verkostojen yhteyden yhteen vuokraajaan. Lisä tietoja on Ohje aiheessa [verkko siirto: usean Yammer-verkoston kokoaminen](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Vaihtoehtoisesti voit pakottaa Yammerin käyttö oikeuden estämään käyttäjiä Yammerista, jos heillä ei ole käyttö oikeutta. Lisä tietoja on Ohje aiheessa [Yammer-käyttö oikeuksien hallinta Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)-sovelluksessa.
4. Valvo lopuksi vanhojen Yammer-verkostojen käyttäjä luetteloa ja Keskeytä vanhat käyttäjät. On suositeltavaa keskeyttää (poistaa käytöstä) käyttäjät niiden poistamisen sijaan, koska poisto on peruuttamaton. Lisä tietoja on Ohje aiheessa [Yammer-käyttäjien valvonta Office 365-verkoissa](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) ja [käyttäjien poistaminen](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Määrittämällä Yammerin näiden vaiheiden avulla voit myös määrittää Yammer-verkoston Microsoft 365-ohjelman alkuperäistä tilaa varten. Lisä tietoja on Ohje aiheessa [Yammer-verkoston määrittäminen Microsoft 365-tila uksen alkuperäistä tilaa](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode)varten.