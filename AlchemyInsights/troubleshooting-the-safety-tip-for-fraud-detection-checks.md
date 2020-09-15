---
title: Vian määritys suojaus vihjeestä petosten havaitsemisen tarkistukset
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658407"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Vian määritys suojaus vihjeestä petosten havaitsemisen tarkistukset

Jos saat turva vihjeen, jossa lukee "lähettäjä ei onnistunut huijausten havaitsemisessa, eikä se ehkä ole", lähettäjä ei voinut siirtää DKIM-tai SPF-todennus tarkistuksia. Paras tapa korjata tämä on se, että lähettäjä valtuuttaa itsensä. Jos lähettäjä lähettää viestin puolestasi, sinun on valtuutettava heidät lisäämällä lähettäjän IP-osoite SPF-tietueeseen.
  
Lisä tietoja [on kohdassa punaisen (epäilyttävän) suojaus vihjeen vian määritys petosten havaitsemis tarkistuksissa](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .
  
Seuraavassa on joitakin muita linkkejä, joista voi olla apua:
  
- [Tietoja siitä, miten Microsoft käyttää SPF (lähettäjän Policy Framework)-järjestelmää tietojen väärentämisen estämiseen](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [SPF-osoitteen määrittäminen estämään tietojen väärentämisen estäminen](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
