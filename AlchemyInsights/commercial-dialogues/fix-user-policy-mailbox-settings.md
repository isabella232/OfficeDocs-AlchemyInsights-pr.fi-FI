---
title: Käyttäjäkäytännön tai postilaatikon asetusten korjaukset
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: fecc52bea66e0aed709a8995d2509f4432c09482459aa575d29e4c7551375211
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034715"
---
# <a name="fix-user-policymailbox-settings"></a>Käyttäjäkäytännön tai postilaatikon asetusten korjaukset

Postilaatikon roskapostiasetukset vaikuttavat tähän viestiin. Voit tarkistaa asetukset seuraavasti:

1. Käynnistä Exchange hallintaliittymä. Lisätietoja on kohdassa [Exchange hallintaliittymän avaaminen.](https://go.microsoft.com/fwlink/?linkid=2101432)
2. Suorita tämä komento (käyttämällä käyttäjän sähköpostiosoitetta):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Tarkista, onko lähettäjän sähköpostiosoite osa luotettuja **lähettäjiäAndDomains** tai **BlockedSendersAndDomains.** Jos sähköpostiosoite on jossakin luettelossa, se on ehkä poistettava. Lisätietoja on kohdassa [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
