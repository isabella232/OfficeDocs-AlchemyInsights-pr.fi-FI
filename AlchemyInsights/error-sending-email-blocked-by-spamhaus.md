---
title: Virhe lähetettäessä sähkö postia, jonka SpamHaus on torjunut
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783800"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Virhe lähetettäessä sähkö postia: asiakas isäntä on torjunut Spamhausin avulla

Viestin lähettänyt IP-osoite on [Spamhausin](https://go.microsoft.com/fwlink/p/?linkid=123245)omistama estettyjen luettelossa. Syitä, joiden vuoksi spamhaus on saattanut estää, ovat vaarantuneet asiakkuudet, luvatut koneet, jotka jakavat julkisen IP-osoitteen ja Internet-palveluntarjoajan käytännöt. Mahdollisia korjauksia ovat seuraavat:
  
- Jos haluat estää saapuvat viestit, joissa voit hallita lähde Sähkö posti palvelinta, sinun on määritettävä syy ja poistettava lohko Spamhausin verkkosivustosta.

- Estettyjen saapuvien viestien osalta, joihin lähde-IP-osoite kuuluu jollekulle muulle, osoitteen omistajan on poistettava lohko Spamhausin verkkosivustosta. Jos IP-osoite on käytäntöjen esto luettelossa (PBL), omistaja voi määrittää eri staattisen IP-osoitteen tai poistaa osoitteen PBL-tiedostosta.

- Voit saada tämän virhe sanoman, kun sähkö posti viesti on kytketty Microsoft-toimi alueelta, jos viestit reititetään kolmannen osapuolen palvelun kautta. Voit etsiä torjutun IP-osoitteen omistajan WHOIS-haku työkalun avulla.
