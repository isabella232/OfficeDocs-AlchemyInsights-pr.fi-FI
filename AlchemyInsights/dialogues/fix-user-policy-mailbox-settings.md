---
title: Käyttäjäkäytännön/postilaatikon asetusten ratkaiseminen
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
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694177"
---
# <a name="fix-user-policymailbox-settings"></a>Käyttäjäkäytännön/postilaatikon asetusten ratkaiseminen

Tämä viesti vaikuttaa postilaatikon roskapostiasetuksiin. Voit tarkistaa asetukset seuraavasti:

1. Käynnistä Exchange-hallintaliittymä. Lisätietoja on ohjeaiheessa [Exchange-hallintaliittymän avaaminen.](https://go.microsoft.com/fwlink/?linkid=2101432)
2. Suorita tämä komento (käyttäjän sähköpostiosoitteella):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Tarkista, onko lähettäjän sähköpostiosoite osa **TrustedSendersAndDomains-** tai **BlockedSendersAndDomains-toimialueita.** Jos sähköpostiosoite on jossakin luettelossa, se on ehkä poistettava. Lisätietoja on kohdassa [Set-MailboxJunkEmailConfiguration.](https://go.microsoft.com/fwlink/?linkid=2101047)
