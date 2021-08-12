---
title: Huijausten turvallisuusvihje vianmääritys
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
ms.openlocfilehash: c7ee1fcc887a3221b5f2acda1aa6ae6beb03cb96686d4ecb7828a02f8ff48302
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955963"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Huijausten turvallisuusvihje vianmääritys

Jos saat virhekoodin turvallisuusvihje jossa lukee "Lähettäjä ei läpäisynyt tunnistustarkistuksemme etkä välttämättä ole se, jonka he näyttävät olevan", lähettäjä ei läpäisynyt DKIM- tai SPF-todennustarkistuksia. Paras tapa ratkaista tämä on se, että lähettäjä voi valtuuttaa itsensä. Jos lähettäjä lähettää viestejä puolestasi, sinun on valtuuttava lähettäjä lisäämällä lähettäjän IP-osoite SPF-tietueeseen.
  
Katso [lisätietoja ohjeista turvallisuusvihje (epäilyttävän)](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) punaisen (epäilyttävän) määrityksen vianmääritys.
  
Seuraavassa on joitakin muita linkkejä, joista voi olla apua:
  
- [Miten Microsoft käyttää SPF (Sender Policy Framework) -kehystä osoitetilemisen estämiseksi](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [SPF:n määritäminen estämään väärentäminen](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
