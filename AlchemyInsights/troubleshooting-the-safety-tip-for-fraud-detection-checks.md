---
title: Petosten havaitsemisen tarkistusten turvallisuusvihjeen vianmääritys
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
ms.openlocfilehash: 61159391f7a9876750cd7fefc40c54054fb9bec9
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759509"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Petosten havaitsemisen tarkistusten turvallisuusvihjeen vianmääritys

Jos saat turvallisuusvihjeen, jossa lukee "Lähettäjä ei läpäissyt petosten havaitsemisen tarkistuksia ja ei välttämättä ole se, kuka ne näyttävät olevan", lähettäjä ei läpäissyt joko DKIM- tai SPF-todennustarkistuksia. Paras tapa ratkaista tämä on, että lähettäjä valtuuttaa itsensä. Jos lähettäjä lähettää puolestasi, sinun on valtuutettava hänet lisäämällä lähettäjän IP-osoite SPF-tietueeseen.
  
Lisätietoja [on ohjeaiheessa Punaisen (epäilyttävän) turvallisuusvihjeen vianmääritys.](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/)
  
Seuraavassa on joitakin muita linkkejä, jotka voivat auttaa:
  
- [Microsoftin huijausten estäminen lähettäjän käytäntökehyksen (SPF) avulla](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [SPF:n määrittäminen estämään väärentäminen](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
