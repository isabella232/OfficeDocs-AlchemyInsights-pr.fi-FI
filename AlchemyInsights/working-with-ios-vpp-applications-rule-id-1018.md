---
title: IOS VPP sovellusten säännön tunnus 1018 käsitteleminen
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 58471f22ce78be1b40d3330a76a92d811819849d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/28/2019
ms.locfileid: "35364846"
---
# <a name="working-with-ios-vpp-applications"></a>IOS VPP-sovellusten käyttäminen

Lue lisätietoja toiminnot, rajoitukset ja toimenpiteet [iOS apps ostaa aseman osto - ohjelma on Microsoft Intune – hallinta](https://docs.microsoft.com/intune/vpp-apps-ios) Apple aseman osto-ohjelma ja tuki-Microsoft Intune hyödyntää.
  
 **Ongelmista:** ”Oma käyttäjille osoitettuja iOS VPP app, mutta asennus epäonnistui”.
  
- Näin voi käydä, jos yhden VPP-tunnusta käytetään useita kannettavan laitteen hallinnan palveluntarjoajien kautta. Apple-VPP-tunnuksia voi käyttää vain yksi toimittaja. Jos käytit VPP-tunnuksen kanssa useita tarjoajia, Lataa uudelleen Intune tunnuksen.

- Asennus saattaa epäonnistua myös, jos asennusten kokonaismäärä ylitä käyttöoikeuksien määrää. Voit tarkastella käyttöoikeuksiasi käyttöraportteja, siirry **Intune Mobile apps** \> **App-käyttöoikeudet** -sivulla. Lisätietoja vapauttaa lisenssejä käyttää, on [Tässä artikkelissa.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
