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
ms.openlocfilehash: d0ef27e7c03eb8bcd9de74c58a5e0398d8892a6eb0ab50944b3c2201247fa0b8
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/11/2021
ms.locfileid: "57889215"
---
# <a name="active-directory-not-syncing"></a>Active Directory ei synkronoidu

Jos saat synkronointivirheitä, kuten "ei viimeaikaista synkronointia", tai huomaat hakemistosynkronoinnin tilan Office-hallintaportaalissa, jossa lukee "Viimeksi synkronoitu yli kolme päivää sitten", AADConnectin asetukset voivat olla virheellisiä tai käyttöoikeudet eivät riitä synkronoinnin suorittamiseen.  

AADConnectin uudelleenasentaminen pika-asetusten avulla voi ratkaista ongelman nopeasti:

1. [Lataa uusin AADConnect-versio.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Noudata pika-asennuksen ohjeita.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

Azure AD Connect täytyy asentaa Windows Server 2012:een tai tätä uudempaan. Tämän palvelimen täytyy olla liitetty toimialueeseen. Se voi olla toimialueen ohjauskone tai jäsenpalvelin. Täydellinen luettelo Azure AD:n Näyttöyhteys ja edellytyksistä on kohdassa Azure AD:n käytön [edellytykset Näyttöyhteys.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

Lisätietoja AADConnect -palvelutileistä on kohdassa [Azure AD Näyttöyhteys: Tilit ja käyttöoikeudet.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)
