---
title: Teams-apuohjelman lisääminen Maciin
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582067"
---
# <a name="teams-add-in-for-mac"></a>Teams-apuohjelman lisääminen Maciin

Voit tehdä vianmäärityksen Teams-apuohjelman Mac-käyttöjärjestelmän käyttäjille seuraavasti:

**Vaihe 1:** Jos käytössäsi on Exchange yhdistelmäympäristö (2016 CU3 tai uudempi), varmista Test-HMA.ps1-työkalun avulla, että moderni yhdistelmä varmennus on määritetty oikein. Lisätietoja on kohdassa Modernin yhdistelmäympäristön [todentamisen määrityksen Outlook iOS- ja Android-versioille.](https://aka.ms/TestHMAEAS)  

**Huomautus** Käytä UPN-osoitemuotoa (esimerkiksi [username@contoso.com](mailto:username@contoso.com)), älä toimialue\käyttäjänimi. Voit tehdä tämän myös käyttäjille, joilla on Exchange Online postilaatikoita.

**Vaihe 2:** Käyttäjän täytyy valita **TyökalutTilit...**  >   ja Outlook for Mac ja etsi ja valitse tili. Varmista, että käyttäjänimi on upn-muodossa (esimerkiksi [username@contoso.com).](mailto:username@contoso.com)

**Vaihe 3:** Varmista, että käyttäjällä on Microsoft Teams käyttöoikeus. Käyttäjän on käytettävä Office 365 for Mac -tilausta, tuoteversiota 16.24 tai uudempaa versiota.