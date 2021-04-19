---
title: SMTP-todennusongelmien ratkaiseminen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826412"
---
# <a name="solving-smtp-authentication-issues"></a>SMTP-todennusongelmien ratkaiseminen

Jos saat virheilmoituksia 5.7.57 tai 5.7.3, kun yrität lähettää SMTP-sähköpostia ja todentaa sen asiakasohjelmalla tai sovelluksella, tarkista muutama asia:

- Todennettu SMTP-lähetys on ehkä poistettu käytöstä vuokraajassa tai postilaatikossa, jota yrität käyttää (tarkista molemmat asetukset). Lisätietoja on kohdassa Todennettua [SMTP-lähetystä koskevan todennuksen ottaminen käyttöön tai poistaminen käytöstä.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)

- Tarkista, [onko Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) otettu käyttöön vuokraajassa; Jos se on käytössä, SMTP-todennus perustodennuksella (tunnetaan myös nimellä vanha; tämä käyttää käyttäjänimeä ja salasanaa) epäonnistuu.
