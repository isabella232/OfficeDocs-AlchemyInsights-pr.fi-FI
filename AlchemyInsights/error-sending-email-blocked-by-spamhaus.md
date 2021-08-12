---
title: Virhe SpamHausin estämiä sähköpostiviestejä lähetettäessä
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8372032e19bd2ebaf3ba8cc8e87f19ef3e2edf1e607b1739a919f6dcc443cd97
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946725"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Virhe sähköpostin lähettämisessä: Asiakkaan isäntä estetty Spamhausin avulla

Viestin lähettänyt IP-osoite on [Spamhausin](https://go.microsoft.com/fwlink/p/?linkid=123245)omistamassa estoluettelossa. Spamhausin estämisen syitä ovat mm. vaarantunut tili, vaarantunut kone, joka jakaa julkisen IP-osoitteen, sekä Internet-palveluntarjoajan käytännöt. Mahdollisia korjauksia ovat seuraavat:
  
- Jos saapuvat viestit ovat estettyjä, kun hallitset lähdesähköpostipalvelinta, sinun on määritettävä syy ja poistettava esto Spamhaus-sivustosta.

- Jos saapuvat viestit on estetty ja IP-lähdeosoite kuuluu jollekulle muulle, osoitteen omistajan on poistettava esto Spamhaus-sivustosta. Jos IP-osoite on PBL-käytännön estoluettelossa, omistaja voi määrittää toisen staattisen IP-osoitteen tai poistaa osoitteen PBL:sta.

- Jos kyse on Microsoftiin yhdistetystä toimialueestasi estetyt lähtevät viestit, voit saada tämän virheen, jos viestit reititetaan kolmannen osapuolen palvelun kautta. Voit etsiä estettyjen IP-osoitteiden omistajan WHOIS-hakutyökalun avulla.
