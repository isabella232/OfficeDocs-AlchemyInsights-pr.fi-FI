---
title: Kalenterin käyttö oikeudet
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: cfee520e26587c0a649c08084853c31232d027f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748790"
---
# <a name="calendar-permissions"></a>Kalenterin käyttö oikeudet

Käyttäjät voivat muuttaa oman kalenterin käyttö oikeuksiaan Outlookin verkko versiossa tai muissa asiakkaissa, mutta sinun on ehkä tutkittava ne myös järjestelmänvalvojana.  
Exchange PowerShellin cmdlet-toiminnolla näet käyttö oikeuden käyttäjän kalenteriin:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Lisä tietoja on seuraavissa artikkeleissa:

- [Get-Mailoff-kansion käyttö oikeudet](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Asetukset-Mailposti kansion käyttö oikeudet](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Lisää-Mailposti kansion käyttö oikeus](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Kalenterin käyttö oikeuksia käytetään kalenterien jakamiseen, jos haluat lisä tietoja Outlook-kalenterin jakamisesta, tutustu seuraaviin artikkeleihin:

- [Outlook-kalenterin jakaminen muiden kanssa](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Kalenterin jakaminen Outlookin verkko versiossa yrityksille](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Voit suorittaa kalenterin käyttö oikeuksien vian määrityksen [tuki-ja palautus avustaja](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) -työkalulla.