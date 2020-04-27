---
title: Postilaatikon automaattisten vastausten määrittäminen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 4ffe8d77dad7db5fd5806fe879cf4934e5ca7c4a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2020
ms.locfileid: "43788879"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Käyttäjän postilaatikon automaattisten vastausten määrittäminen

**Menetelmä 1**

1. Kirjaudu sisään Microsoft 365 -portaaliin.

2. Siirry kohtaan **Käyttäjät > Aktiiviset käyttäjät** (tai **Ryhmät > Jaetut postilaatikot**, jos määrität jaetun postilaatikon).

3. Valitse käyttäjä, jolla on Microsoft Exchange -postilaatikko.

4. Siirry oikealla olevassa pikaikkunavalikossa kohtaan **Sähköpostiasetukset > Automaattiset vastaukset** (jos kyseessä on jaettu postilaatikko, valitse pikaikkunavalikossa **Automaattiset vastaukset**).

**Menetelmä 2**

1. Kirjaudu sisään Microsoft 365 -hallintaportaaliin järjestelmänvalvojan tunnistetiedoilla.

2. Laajenna **Hallintakeskukset** ja valitse sitten **Exchange**.

3. Valitse oikeassa yläkulmassa oleva kuva, valitse **Toinen käyttäjä** ja valitse sitten käyttäjäpostilaatikko, jonka haluat muuttaa.

4. Valitse vasemmalla puolella **Asetukset**, valitse **Järjestä sähköposti** ja valitse sitten **Automaattiset vastaukset.**

**Menetelmä 3**

Suorita seuraava cmdlet-komento Exchange Online PowerShellissä:

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

Lisätietoja tästä cmdlet-komennosta on kohdassa [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
