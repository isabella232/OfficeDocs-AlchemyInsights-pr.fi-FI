---
title: Active Directory ei synkronoidu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 4bfbe6b2dd9a2112f0cb7af0d6e7a46693bc70680895fd674ddb0332b7071797
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53937098"
---
# <a name="active-directory-not-syncing"></a>Active Directory ei synkronoidu

Jos saat synkronointivirheitä, kuten "ei viimeaikaista synkronointia", tai huomaat hakemistosynkronoinnin tilan Office-hallintaportaalissa, jossa lukee "Viimeksi synkronoitu yli kolme päivää sitten", AADConnectissa voi olla virheellisiä asetuksia tai liian vähän käyttöoikeuksia synkronoinnin suorittamiseen.  

AADConnectin uudelleenasentaminen pika-asetusten avulla voi ratkaista ongelman nopeasti:

1. [Lataa uusin AADConnect-versio.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Noudata pika-asennuksen ohjeita.](/azure/active-directory/hybrid/how-to-connect-install-express)

Azure AD Connect täytyy asentaa Windows Server 2012:een tai tätä uudempaan. Tämän palvelimen täytyy olla liitetty toimialueeseen. Se voi olla toimialueen ohjauskone tai jäsenpalvelin. Täydellinen luettelo Azure AD-Näyttöyhteys ja edellytyksistä on kohdassa Azure AD Näyttöyhteys: n [edellytykset.](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

Lisätietoja AADConnect -palvelutileistä on kohdassa [Azure AD Näyttöyhteys: Tilit ja käyttöoikeudet.](/azure/active-directory/hybrid/reference-connect-accounts-permissions)
