---
title: Korjaa sähköpostin toimitus ongelmat postijärjestelmän käynnistämät yleisiin kansioihin
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 900b6cc2765937ee005c7e7dce5d33bbdf582601
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752665"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Korjaa sähköpostin toimitus ongelmat postijärjestelmän käynnistämät yleisiin kansioihin

Jos Ulkoiset lähettäjät voi lähettää viestejä, mail käytössä yleisissä kansioissa ja lähettäjien, näyttöön tulee virhesanoma: **(550 5.4.1) ei löytynyt**, Tarkista sähköposti toimialue on yleinen kansio on määritetty sisäinen relay toimialueen sijaan hallitseva toimialue:

1. Avaa [Exchange-hallintakeskukseen (AKV)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Siirry **postin kulku** \> **hyväksytyt toimialueet**, hyväksytty toimialue ja valitse sitten **Muokkaa**.

3. Ominaisuudet-sivu, avautuu Jos **tärkeimmät**määritetään toimialueen laji, muuta **sisäistä relay** ja valitse sitten **Tallenna**.

Jos Ulkoiset lähettäjät tulee virhe, **sinulla ei ole oikeuksia (550 5.7.13)**, [Exchange Online-PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) julkisessa kansiossa anonyymeille käyttäjille oikeudet suorittamalla seuraavan komennon:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Esimerkiksi `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Ulkoiset käyttäjät voivat lähettää sähköpostia tähän yleiseen kansioon, Lisää CreateItems käyttöä oikealle anonyymi käyttäjä. Esimerkiksi `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
