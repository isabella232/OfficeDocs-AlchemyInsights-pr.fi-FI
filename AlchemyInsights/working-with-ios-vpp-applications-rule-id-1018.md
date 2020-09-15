---
title: IOS:n VPP-sovellus säännön tunnuksen 1018 käyttö
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
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688943"
---
# <a name="working-with-ios-vpp-applications"></a>IOS:n VPP-sovellusten käyttö

Lue [, miten voit hallita Microsoft Intunen kautta ostettuja iOS-sovelluksia](https://docs.microsoft.com/intune/vpp-apps-ios) , joiden avulla saat tietoa ominaisuuksista, rajoitteista ja vaiheista, joilla voit hyödyntää Apple-määrä osto ohjelmaa ja sitä tukevia tietoja Microsoft Intunella.
  
 **Yleisiä ongelmia:** "Määritin käyttäjälleni iOS-VPP-sovelluksen, mutta asennus epäonnistui."
  
- Näin voi käydä, jos yksittäinen VPP-tunnus on käytössä useissa mobiililaitteiden hallinta palveluissa. Applen VPP-tunnuksia voi käyttää vain yhden palveluntarjoajan kanssa. Jos käytit VPP-tunnusta useiden palveluntarjoajien kanssa, sinun on ladattava tunnus uudelleen Intuneen.

- Asennus voi epäonnistua myös, jos asennusten kokonaismäärä ylittää käyttö oikeuksien luku määrän. Jos haluat tarkastella käyttö oikeuksia, siirry **Intune-mobiilisovellusten** \> **sovelluksen käyttö oikeudet** -sivulle. Katso lisä tietoja käyttö oikeuksien hankkimisesta käytöstä [tässä artikkelissa.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
