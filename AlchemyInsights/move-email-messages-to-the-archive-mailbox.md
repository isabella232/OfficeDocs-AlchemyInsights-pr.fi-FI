---
title: Siirtää sähköpostiviestejä postilaatikon arkisto
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 37f256ef31402f5139fdd7c2af8f3a6ca9dc3525
ms.sourcegitcommit: 228c986911ecf73217116a5d1fdcd2e89362774e
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/09/2019
ms.locfileid: "31747200"
---
# <a name="move-email-to-the-archive-mailbox"></a>Siirrä sähköposti postilaatikko arkisto
 
1. Vahvista, että **Arkistoi postilaatikko** on käytössä. Jos et arkistoi postilaatikko käyttöön [tämän artikkelin](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) ohjeiden avulla.

2. Voit arkistoida viestit automaattisesti Arkistoi postilaatikko, pidätys tunnisteen **arkistoida Siirrä** -toiminnolla on määritettävä, **kohdistetaan automaattisesti postilaatikon koko (oletus)-merkintä**. Noudata tätä tunnisteen luominen: [tag arkisto oletus](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).
    
3. Lisää **arkisto** tag, että säilytyskäytäntö. Valitse Exchange-hallintakeskukseen **Säilytyskäytännöt** > Lisää **tag arkisto siirtyy** käytäntöön-> **tallentaa**. 
    
4. Nyt [säilytyskäytännön määrittäminen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) tietyn käyttäjän postilaatikkoon. Samaa käytäntöä sovelletaan sekä **ensisijaisen** että **Arkistoi** postilaatikko. 
    
Saatat joutua pakottamaan hallitun kansion avustajan (MFA) ja uusien asetusten käyttäminen käyttäjän postilaatikkoon. Suorittamalla seuraavan komennon käynnistäminen-hallitun kansion avustajan tietyn postilaatikon samalla [yhdistetty EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) : 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Saat lisätietoja arkisto-käytännön määrittämisestä, [Määritä arkistoinnin ja poistamisen käytännön postilaatikoita varten](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

