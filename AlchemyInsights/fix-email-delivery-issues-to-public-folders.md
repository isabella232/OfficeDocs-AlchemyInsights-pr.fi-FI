---
title: Sähköpostin toimitusongelman ratkaiseminen sähköpostia julkisiin kansioihin
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: ff1400f694ae037a8658356af068b4c20b8fa9d9908dafedb90db7bb6859530f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068809"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Sähköpostin toimitusongelman ratkaiseminen sähköpostia julkisiin kansioihin

Jos ulkoiset lähettäjät eivät voi lähettää viestejä sähköpostia käyttävään julkisiin kansioihin ja lähettäjät saavat virhesanoman: sitä ei löytynyt **(550 5.4.1),** tarkista, että yleisen kansion sähköpostitoimialue on määritetty sisäinen välityspalvelun toimialue-toimialueen sijaan:

1. Avaa [Exchange hallintakeskus (EAC).](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. Valitse **Postinkulku** \> **Hyväksytyt toimialueet**, valitse hyväksytty toimialue ja valitse sitten **Muokkaa**.

3. Jos toimialuetyyppi on määritetty avaamaan ominaisuussivulla **Authoritative**, muuta arvoksi Sisäinen **välitys** ja valitse **sitten Tallenna**.

Jos ulkoiset lähettäjät saavat virheilmoituksen, ettei sinulla ole käyttöoikeutta **(550 5.7.13),** suorita seuraava komento [Exchange Online PowerShellissä,](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) niin näet anonyymien käyttäjien käyttöoikeudet yleiskansiossa:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Esimerkiksi `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Jos haluat sallia ulkoisten käyttäjien lähettää sähköpostia tähän julkiseen kansioon, lisää CreateItems-käyttöoikeus suoraan käyttäjälle Anonyymi. Esimerkiksi `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
