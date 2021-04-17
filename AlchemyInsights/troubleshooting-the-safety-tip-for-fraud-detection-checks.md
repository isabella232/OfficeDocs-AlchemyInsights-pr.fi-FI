---
title: Turvallisuusvihjeen vianmääritys huijausten tunnistustarkistuksissa
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834728"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Turvallisuusvihjeen vianmääritys huijausten tunnistustarkistuksissa

Jos saat turvallisuusvihjeen, jossa lukee "Lähettäjä ei ole onnistunut havaitsemaan huijauksiamme, mutta he eivät ehkä ole sitä, keitä he näyttävät olevan", lähettäjä ei läpäisynyt DKIM- tai SPF-todennustarkistuksia. Paras tapa ratkaista tämä on se, että lähettäjä voi valtuuttaa itsensä. Jos lähettäjä lähettää viestejä puolestasi, sinun on valtuuttava lähettäjä lisäämällä lähettäjän IP-osoite SPF-tietueeseen.
  
Lisätietoja [on kohdassa Punaisen (epäilyttävän) turvallisuusvihjeen vianmääritys huijausten tunnistustarkistuksia](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) varten.
  
Seuraavassa on joitakin muita linkkejä, joista voi olla apua:
  
- [Miten Microsoft käyttää SPF (Sender Policy Framework) -kehystä osoitetilemisen estämiseksi](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [SPF:n määritäminen estämään väärentäminen](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
