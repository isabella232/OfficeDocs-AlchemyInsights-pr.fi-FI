---
title: Virhe lähetettäessä Roskapostin estämiä sähköpostiviestejä
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714255"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Virhe lähetettäessä sähköpostia: Asiakkaan isäntä estetty Roskapostin avulla

Viestin lähettänyt IP-osoite on [Spamhausin](https://go.microsoft.com/fwlink/p/?linkid=123245)omistamassa estoluettelossa. Spamhausin estämisen syitä ovat vaarantuneet tilit, vaarantuneet koneet, joilla on julkinen IP-osoite, sekä Internet-palveluntarjoajan käytännöt. Mahdollisia korjauksia ovat:
  
- Estetyt saapuvat viestit, joissa hallitset lähdesähköpostipalvelinta, sinun on määritettävä syy ja poistettava lohko Spamhaus-sivustosta.

- Estetyt saapuvat viestit, joissa lähteen IP-osoite kuuluu jollekulle muulle, osoitteen omistajan on poistettava lohko Spamhaus-sivustosta. Jos IP-osoite on PBL(Policy Block List) -luettelossa, omistaja voi määrittää toisen staattisen IP-osoitteen tai poistaa osoitteen PBL:stä.

- Jos toimialueeltasi on estettyjä lähteviä viestejä, jotka on yhdistetty Microsoftiin, tämä virhe ilmenee, jos viestit reititetään kolmannen osapuolen palvelun kautta. Voit etsiä estetyn IP-osoitteen omistajan WHOIS-hakutyökalun avulla.
