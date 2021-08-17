---
title: iOS VPP -sovellusten sääntötunnuksen 1018 käyttö
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: f693d12ff0f9c193cba0c6a6802b22d7acd37532c65986e5f6613e18c021f06b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083011"
---
# <a name="working-with-ios-vpp-applications"></a>iOS VPP -sovellusten käyttö

Lue Microsoft Intune:n volyymiosto-ohjelmalla ostettujen [iOS-sovellusten](https://docs.microsoft.com/intune/vpp-apps-ios) hallinta, niin saat lisätietoja Applen volyymiosto-ohjelman käytön ominaisuuksista, rajoituksista ja Microsoft Intune.
  
 **Yleisiä ongelmia:** "Olen määrittänyt käyttäjille iOS VPP -sovelluksen, mutta asennus epäonnistui."
  
- Näin voi käydä, jos yhtä VPP-tunnusta käytetään useissa mobiililaitteiden hallintapalveluntarjoajissa. Applen VPP-tunnuksia voidaan käyttää vain yhden palveluntarjoajan kanssa. Jos käytit VPP-tunnusta useiden palveluntarjoajien kanssa, sinun on ladattava tunnus uudelleen Intuneen.

- Asennus voi epäonnistua myös, jos asennusten kokonaismäärä ylittää käyttöoikeuksien määrän. Jos haluat tarkastella käyttöraporttia käyttöoikeuksistasi, siirry **Intune-mobiilisovellusten** \> **sovelluksen käyttöoikeudet -sivulle.** Lisätietoja käyttöoikeuksien uudelleensyistä on [tässä artikkelissa.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
