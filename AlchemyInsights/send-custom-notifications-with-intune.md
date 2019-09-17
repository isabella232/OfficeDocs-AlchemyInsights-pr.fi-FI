---
title: Mukautettujen ilmoitusten lähettäminen Intune-ominaisuuden avulla
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992310"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Kuinka lähettää mukautettuja ilmoituksia hallittujen iOS-ja Android-laitteiden käyttäjille

Yritys portaali-sovellus käsittelee Intune-sovelluksen mukautetut ilmoitukset käyttäjän laitteessa. Sovellus luo sitten push-ilmoituksen kyseiselle laitteelle.

Seuraavat ovat laitteen edellytyksiä, jotka tukevat mukautettujen ilmoitusten vastaanottoa, ja jotta sovellus luo push-ilmoituksen:

- Laitteessa on oltava asennettuna yritys portaali-sovellus.  

- Laitteen on sallittava yritys portaali-sovelluksen lähettää push-ilmoituksia. Kun sovellus on asennettu tai päivitetty, se kehottaa käyttäjää sallimaan ilmoitukset.

- Android-laitteissa on oltava Google Play-Palvelut asennettuna.

- Laite tulee rekisteröidä Intune.

Lisä tietoja, kuten viestin lähettäminen, on [ominaisuuden dokumentaatiossa](https://docs.microsoft.com/intune/custom-notifications).
