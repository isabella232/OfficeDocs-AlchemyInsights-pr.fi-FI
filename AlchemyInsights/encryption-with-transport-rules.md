---
title: Salaus ja siirtosäännöt
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
- "9002635"
- "5154"
ms.openlocfilehash: dfd77bc83b4b278e3630858f54fdfb109ade2a14
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813865"
---
# <a name="encryption-with-transport-rules"></a>Salaus ja siirtosäännöt

[Exchange-hallintakeskuksessa](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) voit käyttää Office-viestien salaustoimintoja (OME) sähköpostinkulun sääntöihin viestien salaamisen käynnistämiseksi. Valitse siirtosäännön ehdossa **Lisää Office 365 -viestin salaus ja sisältösuojaus** -vaihtoehto.

- Saat lisätietoja artikkelista [Postinkulun salaussäännön määrittäminen](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- Käytä PowerShellissä [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities)-cmdlet-komentoa ja määritä *ApplyOME*-arvoksi $true.
