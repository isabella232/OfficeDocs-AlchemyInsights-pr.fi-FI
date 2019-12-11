---
title: Yleisten kansioiden käyttö ei onnistu
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
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959492"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook ei voi muodostaa yhteyttä julkisiin kansioihin

Jos yleinen kansio-käyttö ei toimi muutamilla käyttäjillä, kokeile seuraavia:

Muodosta yhteys EXO PowerShelliin ja määritä Defaultpublicfolderposti laatikko ongelman käyttäjä tilille vastaamaan yhtä työn käyttäjä tilistä.

Esimerkki:

Hanki posti laatikon Työkäyttäjä | FT Defaultpublicfolderposti laatikko, Effectivepublicfolderposti laatikko

Set-posti laatikko ProblemUser-Defaultpublicfolderposti laatikon \<arvo edellisestä komennosta>

Odota vähintään yksi tunti, jotta muutos tulee voimaan.