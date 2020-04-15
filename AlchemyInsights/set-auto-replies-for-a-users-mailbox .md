---
title: Käyttäjän postilaatikon automaattisten vastausten määrittäminen
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
ms.openlocfilehash: e3cc01298c10fd3ba21327a7fb5cc5396d0ad74d
ms.sourcegitcommit: 23e5b94f1758bfe202008384e300b81816975375
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/14/2020
ms.locfileid: "43506457"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Käyttäjän postilaatikon automaattisten vastausten määrittäminen

**Menetelmä 1**

1. Kirjaudu sisään Office 365 -portaaliin.

2. Siirry kohtaan **Käyttäjät > Aktiiviset käyttäjät** (tai **Ryhmät > Jaetut postilaatikot**, jos määrität jaetun postilaatikon).

3. Valitse käyttäjä, jolla on Microsoft Exchange -postilaatikko.

4. Siirry oikealla olevassa pikaikkunavalikossa kohtaan **Sähköpostiasetukset > Automaattiset vastaukset** (jos kyseessä on jaettu postilaatikko, valitse pikaikkunavalikossa **Automaattiset vastaukset**).

**Menetelmä 2**

1. Kirjaudu sisään Office 365 -hallintaportaaliin järjestelmänvalvojan tunnistetiedoilla.

2. Laajenna **Hallintakeskukset** ja valitse sitten **Exchange**.

3. Valitse oikeassa yläkulmassa oleva kuva, valitse **Toinen käyttäjä** ja valitse sitten käyttäjäpostilaatikko, jonka haluat muuttaa.

4. Valitse vasemmalla puolella **Asetukset**, valitse **Järjestä sähköposti** ja valitse sitten **Automaattiset vastaukset.**

**Menetelmä 3**

Suorita seuraava cmdlet-komento Exchange Online PowerShellissä:

PowerShellCopy

    Set-MailboxAutoReplyConfiguration

Lisätietoja tästä cmdlet-komennosta on kohdassa [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
