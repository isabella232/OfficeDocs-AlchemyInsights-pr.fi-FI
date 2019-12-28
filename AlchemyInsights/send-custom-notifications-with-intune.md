---
title: Mukautettujen ilmoitusten lähettäminen Intune-ominaisuuden avulla
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886854"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Kuinka lähettää mukautettuja ilmoituksia hallittujen iOS-ja Android-laitteiden käyttäjille

Yritys portaali-sovellus käsittelee Intune-sovelluksen mukautetut ilmoitukset käyttäjän laitteessa. Sovellus luo sitten push-ilmoituksen kyseiselle laitteelle.

Seuraavat ovat laitteen edellytyksiä, jotka tukevat mukautettujen ilmoitusten vastaanottoa, ja jotta sovellus luo push-ilmoituksen:

- Laitteessa on oltava asennettuna yritys portaali-sovellus.  

- Laitteen on sallittava yritys portaali-sovelluksen lähettää push-ilmoituksia. Kun sovellus on asennettu tai päivitetty, se kehottaa käyttäjää sallimaan ilmoitukset.

- Android-laitteissa on oltava Google Play-Palvelut asennettuna.

- Laite tulee rekisteröidä Intune.

Lisä tietoja, kuten viestin lähettäminen, on [ominaisuuden dokumentaatiossa](https://docs.microsoft.com/intune/custom-notifications).
