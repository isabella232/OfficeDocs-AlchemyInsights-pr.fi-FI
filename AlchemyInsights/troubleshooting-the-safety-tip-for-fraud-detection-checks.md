---
title: Petostenhavaitsemistarkistusten turvallisuusvihjeen vianmääritys
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 74913492a086de688067d588e95dd87e6946743b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44504980"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Petostenhavaitsemistarkistusten turvallisuusvihjeen vianmääritys

Jos saat turvallisuusvihjeen, jossa lukee "Lähettäjä ei läpäissyt petosten havaitsemistarkistuksia eikä ehkä ole sitä, kuka ne näyttävät olevan", lähettäjä ei läpäissyt DKIM- tai SPF-todennustarkistuksia. Paras tapa ratkaista tämä on, että lähettäjä valtuuttaa itsensä. Jos lähettäjä lähettää sen puolestasi, sinun on valtuutettava se lisäämällä lähettäjän IP-osoite SPF-tietueeseesi.
  
Lisätietoja on [ohjeaiheessa Petosten havaitsemisen vianmääritys punaisen (epäilyttävän) turvallisuusvihjeen](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) vianmääritys.
  
Seuraavassa on joitakin muita linkkejä, jotka voivat auttaa:
  
- [Microsoftin tapa estää väärentäminen lähettäjän käytäntökehyksellä (SPF)](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [SPF:n määrittäminen estämään väärentäminen](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
