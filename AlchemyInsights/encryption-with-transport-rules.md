---
title: Salaus ja siirtosäännöt
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 3f16c7e7be99a50cd57f47ea2801b3022c4aec95
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915085"
---
# <a name="encryption-with-transport-rules"></a>Salaus ja siirtosäännöt

[Exchange-hallintakeskuksessa](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) voit käyttää Office-viestien salaustoimintoja (OME) sähköpostinkulun sääntöihin viestien salaamisen käynnistämiseksi. Valitse siirtosäännön ehdossa **Lisää Office 365 -viestin salaus ja sisältösuojaus** -vaihtoehto.

- Saat lisätietoja artikkelista [Postinkulun salaussäännön määrittäminen](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- Käytä PowerShellissä [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities)-cmdlet-komentoa ja määritä *ApplyOME*-arvoksi $true.
