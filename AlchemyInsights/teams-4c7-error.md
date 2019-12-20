---
title: Teams 4c7-virhe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796088"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7-virhe Microsoft Teamsissa

Tämä virhe ilmenee, koska Microsoft teams edellyttää lomakkeiden todennusta. Kun otat käyttöön Active Directory Federation Servicesin (AD FS), lomakkeiden todennus ei oletusarvoisesti ole käytössä intranetissä. Jos Windowsin integroitu todennus epäonnistuu, sinua kehotetaan Kirjautu maan sisään käyttämällä lomakkeiden todennusta.

Voit ratkaista tämän ongelman ottamalla lomakkeiden todennuksen käyttöön käyttämällä MMC (AD FS Microsoft Management Console)-laajennusta tieto koneessa, jossa on Active Directoryn paikallinen kopio. Voit tehdä tämän seuraavasti: 

1. Siirry siirtymis ruudussa **todennus käytäntöihin**.
2. Valitse tiedot-ruudun **toiminnot** -kohdasta **Muokkaa yleistä ensisijaista todennusta**.
3. Valitse **intranet** -väli lehdestä **lomakkeiden todennus**.
4. Valitse **OK** (tai **Käytä**).