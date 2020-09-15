---
title: Teamsin 4c7-virhe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700200"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7-virhe Microsoft Teamsissa

Tämä virhe johtuu siitä, että Microsoft teams edellyttää lomakkeiden todennusta. Kun otat käyttöön Active Directory-liittoutumis palveluja (AD FS), lomakkeiden todennus ei ole oletusarvoisesti käytössä intranetiin. Jos Windowsin integroitu todennus epäonnistuu, sinua pyydetään Kirjautu maan sisään käyttämällä lomakkeiden todennusta.

Ratkaise ongelma ottamalla käyttöön lomakkeiden todentaminen käyttämällä Microsoft Management Console (MMC)-laajennusta tieto koneessa, jossa on paikallinen kopio Active Directorysta. Voit tehdä tämän seuraavasti: 

1. Etsi siirtymis ruudussa **todennus käytännöt**.
2. Valitse tieto ruudun **toiminnot** -kohdassa **Muokkaa yleistä päätodennusta**.
3. Valitse **intranet** -väli lehdessä **lomakkeiden todennus**.
4. Valitse **OK** (tai **Käytä**).