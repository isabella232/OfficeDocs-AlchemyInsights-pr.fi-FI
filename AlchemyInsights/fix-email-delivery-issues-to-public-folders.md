---
title: Korjaa sähköpostin toimitus ongelmat postijärjestelmän käynnistämät yleisiin kansioihin
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 45665f900014c52e6a920325b0a3b0f6f79fb72d
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32401325"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Korjaa sähköpostin toimitus ongelmat postijärjestelmän käynnistämät yleisiin kansioihin

Jos Ulkoiset lähettäjät voi lähettää viestejä, mail käytössä yleisissä kansioissa ja lähettäjien, näyttöön tulee virhesanoma: **(550 5.4.1) ei löytynyt**, Tarkista sähköposti toimialue on yleinen kansio on määritetty sisäinen relay toimialueen sijaan hallitseva toimialue:

1. Avaa [Exchange-hallintakeskukseen (AKV)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Siirry **postin kulku** \> **hyväksytyt toimialueet**, hyväksytty toimialue ja valitse sitten **Muokkaa**.

3. Ominaisuudet-sivu, avautuu Jos **tärkeimmät**määritetään toimialueen laji, muuta **sisäistä relay** ja valitse sitten **Tallenna**.

Jos Ulkoiset lähettäjät tulee virhe, **sinulla ei ole oikeuksia (550 5.7.13)**, [Exchange Online-PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) julkisessa kansiossa anonyymeille käyttäjille oikeudet suorittamalla seuraavan komennon:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Esimerkiksi `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Ulkoiset käyttäjät voivat lähettää sähköpostia tähän yleiseen kansioon, Lisää CreateItems käyttöä oikealle anonyymi käyttäjä. Esimerkiksi `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
