---
title: Postilaatikon automaattisten vastausten määrittäminen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 85b7e969032607216c948532dcdf83ba09022c7cdfaebce8671c6d2e8fef183d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046605"
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
