---
title: WIX-sivuston käyttäminen Office 365-ostettujen tai hallittujen toimi alueiden kanssa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001516"
- "3582"
ms.openlocfilehash: 522392d41aa8f84f1f4684ccdbd37d68636be07e
ms.sourcegitcommit: cbed17334557c1dfa471623f8d5e735f72e697da
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/28/2020
ms.locfileid: "47300699"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>WIX-sivuston käyttäminen Office 365-ostettujen tai hallittujen toimi alueiden kanssa

- [DNS-tietueiden päivittäminen niin, että sivusto säilyy nykyisessä isännöinti palvelussa](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- WIX-artikkeli "toimi alueen liittäminen WIX:ään osoitin menetelmällä" suosittelee, että käytät (DNS-tietueiden lisäämistä yllä olevaa linkkiä) sen sijaan, että muuttaisit nimi palvelimia, kun käytät Office 365-palvelinta
- Jos haluat edelleen vaihtaa nimi palvelimia WIX:ään, sinun on  [luotava DNS-tietueet WIX:ssä Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Jos toimi alueesi on ostettu Microsoftilta, nimi palvelimia ei voi muuttaa. Jos sinun on muutettava nimi palvelimia, Microsoftin ostettu toimi alue on [siirrettävä toiseen isännöinti palveluun 60 päivän kuluttua](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host) .