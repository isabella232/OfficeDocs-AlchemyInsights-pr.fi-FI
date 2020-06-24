---
title: Kalenterin käyttöoikeudet
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862096"
---
# <a name="calendar-permissions"></a>Kalenterin käyttöoikeudet

Käyttäjät voivat muuttaa omia kalenterioikeuksiaan Outlookin web-sivustolla tai muissa asiakkaissa, mutta järjestelmänvalvojana sinun on ehkä tutkittava myös.  
Exchange PowerShellin cmdlet-liittimessä näytetään käyttäjän kalenterin käyttöoikeudet:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Lisätietoja on seuraavissa ohjeissa:

- [Get-MailboxFolderPermission (Get-MailboxFolderPermission) -kansion](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Aseta mailbox-kansionroisti](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Lisää postilaatikkokansioPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Kalenterin käyttöoikeuksia käytetään kalenterien jakamisessa, jotta saat lisätietoja Outlook-kalenterin jakamisesta, katso seuraavat artikkelit:

- [Outlook-kalenterin jakaminen muiden kanssa](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Kalenterin jakaminen Outlookin verkkoversiossa yrityksille](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Voit tehdä kalenterin käyttöoikeuksien vianmäärityksen [tuki- ja palautusavustajatyökalun](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) avulla.