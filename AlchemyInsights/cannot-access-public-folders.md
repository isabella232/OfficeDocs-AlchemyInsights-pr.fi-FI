---
title: Yleisiä kansioita ei voi käyttää
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891746"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook ei voi muodostaa yhteyttä yleisiin kansioihin

Jos yleisen kansion käyttö ei toimi joillekin käyttäjille, kokeile seuraavaa:

Muodosta yhteys EXO PowerShelliin ja määritä ongelmakäyttäjätilin DefaultPublicFolderMailbox-parametri vastaamaan toimivan käyttäjätilin parametria.

Esimerkki:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox (OletuskansioPostilaatikko),EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox-arvo \<edellisestä komennosta>

Odota vähintään tunti, jotta muutos tulee voimaan.

Jos ongelma ei ratko, toimi [seuraavasti](https://aka.ms/pfcte) yleisen kansion käyttöongelmien vianmäärityksessä Outlookin avulla.