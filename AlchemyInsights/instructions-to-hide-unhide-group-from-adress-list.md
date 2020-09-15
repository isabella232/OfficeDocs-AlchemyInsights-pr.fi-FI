---
title: Piilota/Näytä-ryhmän osoite luettelon ohjeet
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
- "1200024"
- "3161"
ms.openlocfilehash: 1ad9ab294d46ca0fc88a454e3503ddcf80398896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663006"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Piilota Microsoft 365-ryhmä osoite luettelosta (GAL)

Jos haluat piilottaa Microsoft 365-ryhmän Exchange-asiakas ohjelmien (kuten Outlookin tai OWA) osoite luetteloista, käytä seuraavaa komentoa EXO Shell-sovelluksessa:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Jos haluat piilottaa Microsoft 365-ryhmän, joka on näkyvissä Exchange-asiakas ohjelmissa, käytä seuraavaa komentoa EXO Shell-sovelluksessa:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

