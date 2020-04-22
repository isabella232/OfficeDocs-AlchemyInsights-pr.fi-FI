---
title: Sähköpostin toimitusongelmien korjaaminen sähköpostia käyttäviin yleisiin kansioihin
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716349"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Sähköpostin toimitusongelmien korjaaminen sähköpostia käyttäviin yleisiin kansioihin

Jos ulkoiset lähettäjät eivät voi lähettää viestejä sähköpostia käyttäviin yleisiin kansioihin ja lähettäjät saavat virheen: **sitä ei löytynyt (550 5.4.1),** varmista, että yleisen kansion sähköpostitoimialue on määritetty sisäiseksi välitystoimialueeksi hallitsevan toimialueen sijaan:

1. Avaa [Exchange-hallintakeskus (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Siirry **kohtaan Sähköpostin kulku** \> **Hyväksytyt toimialueet**, valitse hyväksytty toimialue ja valitse sitten **Muokkaa**.

3. Jos näyttöön avautuvalla ominaisuudet-sivulla toimialuetyypiksi on määritetty **Hallitseva,** muuta arvoksi **Sisäinen välitys** ja valitse sitten **Tallenna**.

Jos ulkoiset lähettäjät saavat **virheen, johon sinulla ei ole oikeuksia (550 5.7.13),** suorita seuraava komento [Exchange Online PowerShellissä,](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) niin näet anonyymien käyttäjien käyttöoikeudet yleiseen kansioon:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Esimerkiksi `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Jos haluat, että ulkoiset käyttäjät voivat lähettää sähköpostia tähän yleiseen kansioon, lisää CreateItems-käyttöoikeus anonyymille käyttäjälle. Esimerkiksi `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
