---
title: iOS VPP -sovellusten säännön tunnus 1018:n käyttäminen
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719954"
---
# <a name="working-with-ios-vpp-applications"></a>iOS VPP -sovellusten käyttäminen

Lisätietoja Applen volyymiosto-ohjelman ja sen tuen käyttämisestä Microsoft Intunen ominaisuuksissa, rajoitteissa ja vaiheissa on kohdassa [Microsoft Intunen kautta ostettujen iOS-ohjelmien hallinta.](https://docs.microsoft.com/intune/vpp-apps-ios)
  
 **Yleisiä ongelmia:** "Annoin käyttäjillei iOS VPP -sovelluksen, mutta asennus epäonnistui."
  
- Näin voi käydä, jos yhtä VPP-tunnusta käytetään useissa mobiililaitteiden hallintapalveluissa. Applen VPP-tunnuksia saa käyttää vain yhden palveluntarjoajan kanssa. Jos käytit VPP-tunnusta useiden palveluntarjoajien kanssa, sinun on ladattava tunnus uudelleen Intuneen.

- Asennus voi epäonnistua myös, jos asennusten kokonaismäärä ylittää käyttöoikeuksien määrän. Jos haluat tarkastella käyttöraporttia käyttöoikeuksillesi, siirry **Intune Mobile apps** \> **-sovelluksen käyttöoikeudet -sivulle.** Lisätietoja käytössä olesten käyttöoikeuksien palauttamisesta [on tässä artikkelissa.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
